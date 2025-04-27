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
package com.example.containeroptimizer.model;

public class PickSpotResponse {
    private int row;
    private int column;
    private int score;

    public PickSpotResponse(int row, int column, int score) {
        this.row = row;
        this.column = column;
        this.score = score;
    }

    // Getters and Setters
    public int getRow() {
        return row;
    }

    public void setRow(int row) {
        this.row = row;
    }

    public int getColumn() {
