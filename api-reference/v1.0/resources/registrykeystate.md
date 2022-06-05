---
title: Tipo de recurso registryKeyState
description: Contém informações sobre alterações de chave do Registro relacionadas ao alerta e o processo que alterou as chaves do Registro.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a3bdf345c5c34721563dd69c9f3df18695a333a3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900104"
---
# <a name="registrykeystate-resource-type"></a>Tipo de recurso registryKeyState

Namespace: microsoft.graph

Contém informações sobre alterações de chave do Registro relacionadas ao alerta e o processo que alterou as chaves do Registro.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Colméia|registryHive|Um [hive do Registro do Windows](/windows/desktop/sysinfo/registry-hives) : <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>\\HKEY_USERS. Padrão.</li></ul> Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.|
|chave|Cadeia de Caracteres|Chave do Registro atual (ou seja, alterada) (exclui o HIVE).|
|oldKey|Cadeia de Caracteres|Chave do Registro anterior (ou seja, antes da alteração) (exclui o HIVE).|
|oldValueData|Cadeia de Caracteres|Dados de valor da chave do Registro (conteúdo) anteriores (ou seja, antes da alteração).|
|oldValueName|Cadeia de Caracteres|Anterior (ou seja, antes da alteração) do nome do valor da chave do Registro.|
|Operação|registryOperation|Operação que alterou o nome e/ou o valor da chave do Registro. Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.|
|Processid|Int32|ID do processo (PID) do processo que modificou a chave do Registro (os detalhes do processo aparecerão na coleção de alertas 'processos').|
|Valuedata|String|Dados de valor da chave do Registro (conteúdo) atuais (ou seja, alterados).|
|Valuename|Cadeia de Caracteres|Nome do valor da chave do Registro atual (ou seja, alterado)|
|Valuetype|registryValueType|[Tipo de valor da chave do Registro](/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

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

