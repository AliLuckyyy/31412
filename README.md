# 31412
pragma solidity ^0.8.0;

contract DailyCalendar {
    mapping(uint256 => string) public events;

    function addEvent(uint256 day, string memory eventDescription) public {
        events[day] = eventDescription;
    }

    function getEvent(uint256 day) public view returns (string memory) {
        return events[day];
    }
}
