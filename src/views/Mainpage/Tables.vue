<script setup>

import AuthorsTable from "../components/AuthorsTable.vue";
import ProjectsTable from "../components/ProjectsTable.vue";
import Tasks from "@/views/Mainpage/TableComponents/Tasks.vue";
import Pagination from "@/views/components/Pagination.vue";
import MonthCalender from "@/views/Calender/MonthCalender.vue";
import Clock from "@/views/Mainpage/RightTopClock.vue";
import RightTopClock from "@/views/Mainpage/RightTopClock.vue";

</script>
<template>
  <div class="py-4 container-fluid">
    <div>
      <!-- Left arrow (fixed) -->
      <a
          class="page-link"
          href="#"
          aria-label="Previous"
          style="position: fixed; left: 20px; top: 50%; transform: translateY(-50%); z-index: 10;"
      >
        <i class="fa fa-angle-left"></i>
        <span class="sr-only">Previous</span>
      </a>

      <!-- Tasks component (scrollable) -->
      <div class="tasks-container mx-5">
        <Tasks />
      </div>

      <!-- Right arrow (fixed) -->
      <a
          class="page-link"
          href="#"
          aria-label="Next"
          style="position: fixed; right: 20px; top: 50%; transform: translateY(-50%); z-index: 10;"
      >
        <i class="fa fa-angle-right"></i>
        <span class="sr-only">Next</span>
      </a>
    </div>
    <div class="tasks-container mx-5">
      <month-calender/>
    </div>
    <div>
      <right-top-clock/>
    </div>

<!--    <div class="row">-->
<!--      <div class="col-12 d-flex justify-content-center">-->
<!--        <Pagination>-->
<!--        </Pagination>-->
<!--      </div>-->
<!--    </div>-->
  </div>
</template>
