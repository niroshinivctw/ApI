# Container Optimizer API

## Overview

A simple Spring Boot microservice for container-routing optimization.
It finds the best spot (lowest score) in the yard map.

## API

### POST `/pickSpot`

**Request Example**:
```json
{
  "yardMap": [
    [5, 8, 9],
    [4, 3, 6],
    [7, 2, 1]
  ]
}
{
  "yardMap": [
    [5, 8, 9],
    [4, 3, 6],
    [7, 2, 1]
  ]
}
package com.example.containeroptimizer.model;

import java.util.List;

public class PickSpotRequest {
    private List<List<Integer>> yardMap;

    // Getter and Setter for yardMap
    public List<List<Integer>> getYardMap() {
        return yardMap;
    }

    public void setYardMap(List<List<Integer>> yardMap) {
        this.yardMap = yardMap;
    }
}
    
