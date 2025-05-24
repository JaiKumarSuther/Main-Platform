<template>
  <div class="select-date-mobile">
    <div class="search-result-container">
      <div class="select-date-header">
        <h2>Select Date</h2>
        <svg
          width="25"
          height="25"
          viewBox="0 0 100 100"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <!-- Circle outline -->
          <circle
            cx="50"
            cy="50"
            r="45"
            stroke="#5A6783"
            stroke-width="4"
          ></circle>

          <!-- Cross line 1 -->
          <line
            x1="35"
            y1="35"
            x2="65"
            y2="65"
            stroke="#5A6783"
            stroke-width="4"
            stroke-linecap="round"
          ></line>

          <!-- Cross line 2 -->
          <line
            x1="65"
            y1="35"
            x2="35"
            y2="65"
            stroke="#5A6783"
            stroke-width="4"
            stroke-linecap="round"
          ></line>
        </svg>
      </div>
      <div class="calendar-container">
        <div class="calendar-dropdown" id="calendarDropdown">
          <div class="calendar-months">
            <!-- Month 1 -->
            <div class="month">
              <table class="calendar">
                <thead>
                  <tr>
                    <th>SU</th>
                    <th>MO</th>
                    <th>TU</th>
                    <th>WE</th>
                    <th>TH</th>
                    <th>FR</th>
                    <th>SA</th>
                  </tr>
                </thead>
              </table>
              <div class="calendar-header">
                <span class="month-name">Aug 2025</span>
              </div>
              <table class="calendar">
                <tbody>
                  <!-- Fill these dynamically -->
                  <tr>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td>1</td>
                    <td>2</td>
                  </tr>
                  <tr>
                    <td>3</td>
                    <td>4</td>
                    <td>5</td>
                    <td>6</td>
                    <td>7</td>
                    <td>8</td>
                    <td>9</td>
                  </tr>
                  <tr>
                    <td>10</td>
                    <td>11</td>
                    <td>12</td>
                    <td>13</td>
                    <td>14</td>
                    <td>15</td>
                    <td>16</td>
                  </tr>
                  <tr>
                    <td>17</td>
                    <td>18</td>
                    <td>19</td>
                    <td>20</td>
                    <td>21</td>
                    <td>22</td>
                    <td>23</td>
                  </tr>
                  <tr>
                    <td>24</td>
                    <td>25</td>
                    <td>26</td>
                    <td>27</td>
                    <td>28</td>
                    <td>29</td>
                    <td>30</td>
                  </tr>
                  <tr>
                    <td>31</td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                  </tr>
                </tbody>
              </table>
            </div>

            <!-- Month 2 -->
            <div class="month">
              <table class="calendar">
                <thead>
                  <tr>
                    <th>SU</th>
                    <th>MO</th>
                    <th>TU</th>
                    <th>WE</th>
                    <th>TH</th>
                    <th>FR</th>
                    <th>SA</th>
                  </tr>
                </thead>
              </table>
              <div class="calendar-header">
                <span class="month-name">Sep 2025</span>
              </div>
              <table class="calendar">
                <tbody>
                  <tr>
                    <td>1</td>
                    <td>2</td>
                    <td>3</td>
                    <td>4</td>
                    <td>5</td>
                    <td>6</td>
                    <td>7</td>
                  </tr>
                  <tr>
                    <td>8</td>
                    <td>9</td>
                    <td>10</td>
                    <td>11</td>
                    <td>12</td>
                    <td>13</td>
                    <td>14</td>
                  </tr>
                  <tr>
                    <td>15</td>
                    <td>16</td>
                    <td>17</td>
                    <td>18</td>
                    <td>19</td>
                    <td>20</td>
                    <td>21</td>
                  </tr>
                  <tr>
                    <td>22</td>
                    <td>23</td>
                    <td>24</td>
                    <td>25</td>
                    <td>26</td>
                    <td>27</td>
                    <td>28</td>
                  </tr>
                  <tr>
                    <td>29</td>
                    <td>30</td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>

          <!-- Control Buttons -->
          <div class="calendar-controls">
            <div>
              <button class="active">Exact date</button>
              <button>+ / - 1 day</button>
              <button>+ / - 2 days</button>
              <button>+ / - 3 days</button>
            </div>
            <button class="add-date-btn">Add date</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
