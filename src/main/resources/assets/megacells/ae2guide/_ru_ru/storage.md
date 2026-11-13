---
navigation:
  title: Хранилища МЕГА
  icon: item_storage_cell_256m
  parent: index.md
  position: 010
categories:
  - megacells
item_ids:
  - cell_component_1m
  - cell_component_4m
  - cell_component_16m
  - cell_component_64m
  - cell_component_256m
  - mega_item_cell_housing
  - mega_fluid_cell_housing
  - mega_chemical_cell_housing
  - mega_source_cell_housing
  - mega_mana_cell_housing
  - mega_experience_cell_housing
  - item_storage_cell_1m
  - item_storage_cell_4m
  - item_storage_cell_16m
  - item_storage_cell_64m
  - item_storage_cell_256m
  - fluid_storage_cell_1m
  - fluid_storage_cell_4m
  - fluid_storage_cell_16m
  - fluid_storage_cell_64m
  - fluid_storage_cell_256m
  - chemical_storage_cell_1m
  - chemical_storage_cell_4m
  - chemical_storage_cell_16m
  - chemical_storage_cell_64m
  - chemical_storage_cell_256m
  - source_storage_cell_1m
  - source_storage_cell_4m
  - source_storage_cell_16m
  - source_storage_cell_64m
  - source_storage_cell_256m
  - mana_storage_cell_1m
  - mana_storage_cell_4m
  - mana_storage_cell_16m
  - mana_storage_cell_64m
  - mana_storage_cell_256m
  - experience_storage_cell_1m
  - experience_storage_cell_4m
  - experience_storage_cell_16m
  - experience_storage_cell_64m
  - experience_storage_cell_256m
  - portable_item_cell_1m
  - portable_item_cell_4m
  - portable_item_cell_16m
  - portable_item_cell_64m
  - portable_item_cell_256m
  - portable_fluid_cell_1m
  - portable_fluid_cell_4m
  - portable_fluid_cell_16m
  - portable_fluid_cell_64m
  - portable_fluid_cell_256m
  - portable_chemical_cell_1m
  - portable_chemical_cell_4m
  - portable_chemical_cell_16m
  - portable_chemical_cell_64m
  - portable_chemical_cell_256m
  - portable_source_cell_1m
  - portable_source_cell_4m
  - portable_source_cell_16m
  - portable_source_cell_64m
  - portable_source_cell_256m
  - portable_mana_cell_1m
  - portable_mana_cell_4m
  - portable_mana_cell_16m
  - portable_mana_cell_64m
  - portable_mana_cell_256m
  - portable_experience_cell_1m
  - portable_experience_cell_4m
  - portable_experience_cell_16m
  - portable_experience_cell_64m
  - portable_experience_cell_256m
  - sky_bronze_ingot
  - sky_bronze_block
  - sky_osmium_ingot
  - sky_osmium_block
---

# MEGA Cells: хранение

<GameScene zoom="8" background="transparent">
  <ImportStructure src="assets/assemblies/drive_cells.snbt" />
  <IsometricCamera yaw="195" pitch="10" />
</GameScene>

## МЕГА [ячейки хранения](ae2:items-blocks-machines/storage_cells.md)

<Row>
  <ItemImage id="mega_item_cell_housing" scale="4" />
  <ItemImage id="item_storage_cell_1m" scale="4" />
  <ItemImage id="item_storage_cell_4m" scale="4" />
  <ItemImage id="item_storage_cell_16m" scale="4" />
  <ItemImage id="item_storage_cell_64m" scale="4" />
  <ItemImage id="item_storage_cell_256m" scale="4" />
</Row>

Как уже упоминалось, <ItemLink id="megacells:accumulation_processor" /> — первый шаг к любой инфраструктуре
MEGA, включая ячейки хранения более высоких уровней. Этот процессор позволяет
развить <ItemLink id="ae2:cell_component_256k" /> *ещё дальше*: от **1M** (эквивалент «1024k») до высшего
уровня **256M**, вместимость которого более чем в *тысячу* раз превышает 256k.

<RecipeFor id="cell_component_1m" />
<RecipeFor id="cell_component_4m" />
<RecipeFor id="cell_component_16m" />
<RecipeFor id="cell_component_64m" />
<RecipeFor id="cell_component_256m" />

Более вместительному хранилищу нужен и более прочный корпус. Для изготовления корпуса
предметной ячейки под новые компоненты M-уровня понадобится ещё немного небесной стали.

<Row>
  <RecipeFor id="mega_item_cell_housing" />
  <Recipe id="cells/standard/item_storage_cell_1m" />
  <Recipe id="cells/standard/item_storage_cell_1m_with_housing" />
</Row>

Для жидкостей и других ресурсов также предусмотрены специальные корпуса. Небесный камень
может образовывать сплавы с другими металлами: например, с медью получается **небесная
бронза** для корпусов жидкостных ячеек. Даже для ресурсов, не рассмотренных в
этом руководстве, MEGA может предоставлять специальную ячейку с собственным типом корпуса.

<Row>
  <ItemImage id="sky_bronze_ingot" scale="4" />
  <ItemImage id="mega_fluid_cell_housing" scale="4" />
  <ItemImage id="fluid_storage_cell_1m" scale="4" />
  <ItemImage id="fluid_storage_cell_4m" scale="4" />
  <ItemImage id="fluid_storage_cell_16m" scale="4" />
  <ItemImage id="fluid_storage_cell_64m" scale="4" />
  <ItemImage id="fluid_storage_cell_256m" scale="4" />
</Row>

<Row>
  <Recipe id="transform/sky_bronze_ingot" />
  <RecipeFor id="mega_fluid_cell_housing" />
</Row>

## МЕГА [портативные ячейки](ae2:items-blocks-machines/storage_cells.md#portable-item-storage)

Как и сам AE2, MEGA предлагает портативные версии всех
своих ячеек, но их повышенная вместимость требует заметно больше энергии.
Поэтому в их рецептах используется <ItemLink id="ae2:dense_energy_cell" /> вместо обычного <ItemLink id="ae2:energy_cell" />.

Эти портативные ячейки поддерживают все [улучшения](ae2:items-blocks-machines/upgrade_cards.md), доступные
обычным портативным МЭ-ячейкам. Однако из-за увеличенного аккумулятора
и высокого энергопотребления обычная <ItemLink id="ae2:energy_card" /> для них недостаточно
мощна. Для этой задачи подходит только <ItemLink id="megacells:greater_energy_card" />.

<Row>
  <RecipeFor id="portable_item_cell_1m" />
</Row>
