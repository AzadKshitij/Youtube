---

database-plugin: basic

---

```yaml:dbfolder
name: new database
description: new description
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 0
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      content_vertical_alignment: align-middle
  published:
    input: checkbox
    accessorKey: published
    key: published
    id: published
    label: published
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: 1
    isSorted: true
    isSortedDesc: false
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  tags:
    input: tags
    accessorKey: tags
    key: tags
    id: tags
    label: tags
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 178
    options:
      - { label: "youtube", value: "youtube", color: "hsl(112, 95%, 90%)"}
      - { label: "100dausofproduct", value: "100dausofproduct", color: "hsl(5, 95%, 90%)"}
      - { label: "2mvideo", value: "2mvideo", color: "hsl(127, 95%, 90%)"}
      - { label: "DS101", value: "DS101", color: "hsl(20, 95%, 90%)"}
      - { label: "shorts", value: "shorts", color: "hsl(300, 95%, 90%)"}
      - { label: "devlog", value: "devlog", color: "hsl(120, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  status:
    input: select
    accessorKey: status
    key: status
    id: Status
    label: status
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Idea", value: "Idea", color: "hsl(307, 95%, 90%)"}
      - { label: "Doing", value: "Doing", color: "hsl(35, 95%, 90%)"}
      - { label: "Done", value: "Done", color: "hsl(305, 95%, 90%)"}
      - { label: "[,Doing]", value: "[,Doing]", color: "hsl(232, 95%, 90%)"}
      - { label: "[,Idea]", value: "[,Idea]", color: "hsl(113, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
config:
  remove_field_when_delete_column: false
  cell_size: compact
  sticky_first_column: true
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 100
  font_size: 16
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: true
  implementation: default
  show_metadata_tags: false
filters:
  enabled: false
  conditions:
```