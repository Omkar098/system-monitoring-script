# system-monitoring-script
top_apps() {
  echo "Top 10 Applications by CPU Usage:"
  ps -eo pid,comm,%cpu,%mem --sort=-%cpu | head -n 11
  echo ""
}
top_mem_apps() {
  echo "Top 10 Applications by Memory Usage:"
  ps -eo pid,comm,%cpu,%mem --sort=-%mem | head -n 11
  echo ""
}
