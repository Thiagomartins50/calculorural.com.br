npm install --save @sentry/react

import * as Sentry from "@sentry/react";

Sentry.init({
  dsn: "https://ee0cdb04677ab306ad946de7a2ff7005@o4512101518868480.ingest.us.sentry.io/4512115746668544",
  dataCollection: {
    // To disable sending user data and HTTP bodies, uncomment the lines below. For more info visit:
    // https://docs.sentry.io/platforms/javascript/guides/react/configuration/options/#dataCollection
    // userInfo: false,
    // httpBodies: []
  }
});

const container = document.getElementById("app");
const root = createRoot(container);
root.render(<App />);

import * as Sentry from '@sentry/react';
// Add this button component to your app to test Sentry's error tracking
function ErrorButton() {
  return (
    <button
      onClick={() => {
        throw new Error('This is your first error!');
      }}
    >
      Break the world
    </button>
  );
}
import * as Sentry from "@sentry/react";

Sentry.init({
  dsn: "https://ee0cdb04677ab306ad946de7a2ff7005@o4512101518868480.ingest.us.sentry.io/4512115746668544",
  dataCollection: {
    // To disable sending user data and HTTP bodies, uncomment the lines below. For more info visit:
    // https://docs.sentry.io/platforms/javascript/guides/react/configuration/options/#dataCollection
    // userInfo: false,
    // httpBodies: []
  }
});

const container = document.getElementById("app");
const root = createRoot(container);
root.render(<App />);
