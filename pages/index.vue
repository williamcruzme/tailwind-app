<template>
  <div>
    <!-- BAD: Using a traditional approach where custom designs require custom CSS -->
    <div class="chat-notification">
      <div class="chat-notification-logo-wrapper">
        <img class="chat-notification-logo" src="/img/chat.svg" alt="ChitChat Logo">
      </div>
      <div class="chat-notification-content">
        <h4 class="chat-notification-title">
          ChitChat
        </h4>
        <p class="chat-notification-message">
          You have a new message!
        </p>
      </div>
    </div>

    <br>

    <!-- GOOD: Using utility classes to build custom designs without writing CSS -->
    <div class="flex max-w-sm p-6 mx-auto bg-white rounded-lg shadow-xl">
      <div class="flex-none">
        <img class="w-12 h-12" src="/img/chat.svg" alt="ChitChat Logo">
      </div>
      <div class="pt-1 ml-6">
        <h4 class="text-xl leading-tight text-gray-900">
          ChitChat
        </h4>
        <p class="leading-normal text-gray-600">
          You have a new message!
        </p>
      </div>
    </div>
  </div>
</template>

<style>
  .chat-notification {
    display: flex;
    max-width: 24rem;
    margin: 0 auto;
    padding: 1.5rem;
    border-radius: 0.5rem;
    background-color: #fff;
    box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
  }
  .chat-notification-logo-wrapper {
    flex-shrink: 0;
  }
  .chat-notification-logo {
    height: 3rem;
    width: 3rem;
  }
  .chat-notification-content {
    margin-left: 1.5rem;
    padding-top: 0.25rem;
  }
  .chat-notification-title {
    color: #1a202c;
    font-size: 1.25rem;
    line-height: 1.25;
  }
  .chat-notification-message {
    color: #718096;
    font-size: 1rem;
    line-height: 1.5;
  }
</style>
