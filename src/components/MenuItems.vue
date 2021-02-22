<template>
  <div class="px-2 space-y-1">
    <a
      href="#"
      :class="isMenuItemActive('all') ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white'"
      class="group flex items-center px-2 py-2 text-sm font-medium rounded-md"
      @click.prevent="handleMenuItem('all')"
    >
      <svg
        class="mr-3 h-6 w-6"
        :class="isMenuItemActive('all') ? 'text-gray-300' : 'text-gray-400 group-hover:text-gray-300'"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 10h16M4 14h16M4 18h16"
        />
      </svg>
      {{ $t('All Feeds') }}
      <span
        v-if="getAllCount > 0"
        class="bg-gray-900 group-hover:bg-gray-800 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full"
      >
        {{ getAllCount }}
      </span>
    </a>

    <a
      href="#"
      :class="isMenuItemActive('favourites') ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white'"
      class="group flex items-center px-2 py-2 text-sm font-medium rounded-md"
      @click.prevent="handleMenuItem('favourites')"
    >
      <svg
        class="mr-3 h-6 w-6"
        :class="isMenuItemActive('all') ? 'text-gray-300' : 'text-gray-400 group-hover:text-gray-300'"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"
        />
      </svg>
      {{ $t('Favourites') }}
      <span
        v-if="getFavouriteCount > 0"
        class="bg-gray-900 group-hover:bg-gray-800 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full"
      >
        {{ getFavouriteCount }}
      </span>
    </a>

    <a
      href="#"
      :class="isMenuItemActive('unread') ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white'"
      class="group flex items-center px-2 py-2 text-sm font-medium rounded-md"
      @click.prevent="handleMenuItem('unread')"
    >
      <svg
        class="mr-3 h-6 w-6"
        :class="isMenuItemActive('all') ? 'text-gray-300' : 'text-gray-400 group-hover:text-gray-300'"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 10h16M4 14h16M4 18h16"
        />
      </svg>
      {{ $t('Unread Articles') }}
      <span
        v-if="getUnreadCount > 0"
        class="bg-gray-900 group-hover:bg-gray-800 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full"
      >
        {{ getUnreadCount }}
      </span>
    </a>

    <a
      href="#"
      :class="isMenuItemActive('read') ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white'"
      class="group flex items-center px-2 py-2 text-sm font-medium rounded-md"
      @click.prevent="handleMenuItem('read')"
    >
      <svg
        class="mr-3 h-6 w-6"
        :class="isMenuItemActive('all') ? 'text-gray-300' : 'text-gray-400 group-hover:text-gray-300'"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        aria-hidden="true"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M8 16l2.879-2.879m0 0a3 3 0 104.243-4.242 3 3 0 00-4.243 4.242zM21 12a9 9 0 11-18 0 9 9 0 0118 0z"
        />
      </svg>
      {{ $t('Recently Read') }}
      <span
        v-if="getReadCount > 0"
        class="bg-gray-900 group-hover:bg-gray-800 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full"
      >
        {{ getReadCount }}
      </span>
    </a>

    <a
      href="#"
      :class="isMenuItemActive('played') ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white'"
      class="group flex items-center px-2 py-2 text-sm font-medium rounded-md"
      @click.prevent="handleMenuItem('played')"
    >
      <svg
        class="mr-3 h-6 w-6"
        :class="isMenuItemActive('all') ? 'text-gray-300' : 'text-gray-400 group-hover:text-gray-300'"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"
        />
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
        />
      </svg>
      {{ $t('Recently Played') }}
      <span
        v-if="getPlayedCount > 0"
        class="bg-gray-900 group-hover:bg-gray-800 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full"
      >
        {{ getPlayedCount }}
      </span>
    </a>

    <a
      href="#"
      :class="isMenuItemActive('saved') ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white'"
      class="group flex items-center px-2 py-2 text-sm font-medium rounded-md"
      @click.prevent="handleMenuItem('saved')"
    >
      <svg
        class="mr-3 h-6 w-6"
        :class="isMenuItemActive('all') ? 'text-gray-300' : 'text-gray-400 group-hover:text-gray-300'"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M8 7H5a2 2 0 00-2 2v9a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-3m-1 4l-3 3m0 0l-3-3m3 3V4"
        />
      </svg>
      {{ $t('Saved articles') }}
      <span
        v-if="getSavedCount > 0"
        class="bg-gray-900 group-hover:bg-gray-800 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full"
      >
        {{ getSavedCount }}
      </span>
    </a>
  </div>
</template>
<script>
import bus from '../services/bus'
import feedMix from '../mixins/feedMix'

export default {
  mixins: [
    feedMix
  ],
  data () {
    return {
      showLess: false
    }
  },
  computed: {
    getAllCount () {
      return this.$store.state.Article.articles.length
    },
    getFavouriteCount () {
      return this.$store.state.Article.articles.filter(article => article.articles.favourite).length
    },
    getUnreadCount () {
      return this.$store.state.Article.articles.filter(article => !article.articles.read).length
    },
    getReadCount () {
      return this.$store.state.Article.articles.filter(article => article.articles.read).length
    },
    getPlayedCount () {
      return this.$store.state.Article.articles.filter(article => article.articles.podcast && article.articles.played).length
    },
    getSavedCount () {
      return this.$store.state.Article.articles.filter(article => article.articles.offline).length
    }
  },
  methods: {
    handleMenuItem (type) {
      bus.$emit('change-article-list', {
        type: 'type-page',
        item: type
      })
    },
    showLessItems () {
      this.showLess = !this.showLess
    }
  }
}
</script>
<style lang="scss" scoped>
.menu-link-clickable {
  cursor: pointer;
}
</style>
