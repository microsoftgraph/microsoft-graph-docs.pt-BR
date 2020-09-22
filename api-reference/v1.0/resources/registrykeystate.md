---
title: tipo de recurso registryKeystate
description: Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eaf1b3ff83a9809b2c283cdad7aef95bd9ca908d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002937"
---
# <a name="registrykeystate-resource-type"></a>tipo de recurso registryKeystate

Namespace: microsoft.graph

Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Hive|registryHive|Uma [seção de registro do Windows](/windows/desktop/sysinfo/registry-hives) : <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE \SAM</li> <li>HKEY_LOCAL_MACHINE \Security</li> <li>HKEY_LOCAL_MACHINE \Software</li> <li>HKEY_LOCAL_MACHINE \System</li> <li>HKEY_USERS \\ . Será.</li></ul> Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.|
|chave|String|Chave de registro atual (ou seja, alterada) (exclui HIVE).|
|oldKey|String|Chave de registro anterior (ou seja, antes da alteração) (exclui HIVE).|
|oldValueData|String|Dados anteriores (ou seja, antes da alteração) dos valores da chave do registro (conteúdo).|
|oldValue|String|Nome do valor da chave anterior (ou seja, antes da alteração).|
|operações|registryOperation|Operação que alterou o nome da chave do registro e/ou o valor. Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.|
|Identificação|Int32|ID de processo (PID) do processo que modificou a chave de registro (os detalhes do processo aparecerão na coleção Alert ' Processes ').|
|valueData|String|Dados de valores de chave de registro (conteúdo) atuais (ou seja, alterados).|
|valueName|String|Nome do valor da chave do registro atual (ou seja, alterado)|
|valueType|registryValueType|[Tipo de valor da chave do registro](/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

