# Refresh Strategies
In Pega, refresh strategies are used to control how frequently the system retrieves data from an external data source to ensure that the information displayed to users is up-to-date. Refresh strategies are particularly important when dealing with data that changes frequently and needs to be refreshed periodically to reflect the latest updates.

**Purpose** 

The primary purpose of refresh strategies is to define how often the system should refresh data from external sources to ensure that it remains current and accurate.

**Configuration** 

Refresh strategies are configured at the data page level in Pega. A data page is a reusable container for holding data retrieved from a data source. By configuring a refresh strategy for a data page, you specify how often the system should reload the data from the source.

**Types of Refresh Strategies**:
   - **Time-based Refresh**: With time-based refresh strategies, you specify a fixed interval at which the system should refresh the data. For example, you might configure a data page to refresh every 5 minutes.
   - **Event-based Refresh**: With event-based refresh strategies, the system triggers a refresh based on specific events or conditions. For example, you might configure a data page to refresh whenever a certain property value changes or when a user performs a specific action.
   - **Manual Refresh**: Manual refresh strategies allow users to manually trigger a refresh of the data by clicking a button or performing some other action in the user interface.

**Caching** 

Refresh strategies work in conjunction with caching mechanisms to optimize performance and reduce the load on external data sources. By caching data locally, the system can serve subsequent requests without having to retrieve the data from the external source again, unless a refresh is explicitly triggered.

**Configuration Options** 

When configuring a refresh strategy for a data page, you can specify various options, such as the refresh interval, conditions for event-based refresh, caching settings, and error handling behavior.

**Best Practices** 

When designing refresh strategies in Pega, it's important to consider factors such as the frequency of data updates, the impact on system performance, and the user experience. You should choose an appropriate refresh strategy based on these considerations to ensure optimal performance and usability.

Overall, refresh strategies play a crucial role in maintaining data freshness and ensuring that users have access to the most up-to-date information in Pega applications. By configuring refresh strategies effectively, you can improve the overall user experience and productivity within your application.