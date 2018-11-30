---
title: tipo de recurso de registryKeyState
description: Contém informações sobre alterações de chave do registro relacionadas ao alerta e o processo que foi alterado as chaves do registro.
ms.openlocfilehash: 37654aab2bf8f0afae0f7ec6ed544aed8634dacc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033808"
---
# <a name="registrykeystate-resource-type"></a>tipo de recurso de registryKeyState

Contém informações sobre alterações de chave do registro relacionadas ao alerta e o processo que foi alterado as chaves do registro.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hive|registryHive|Uma [seção de registro do Windows](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) : <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\SYSTEM</li> <li>HKEY_USERS\\. Padrão.</li></ul> Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.|
|key|String|Chave de registro (ou seja alterado) atual (exclui HIVE).|
|oldKey|String|Anterior (isto é, antes de o alterado) chave do registro (exclui HIVE).|
|oldValueData|String|Anterior (isto é, antes de o alterado) dados do valor da chave do registro (conteúdo).|
|oldValueName|String|Anterior (isto é, antes de o alterado) nome do valor da chave do registro.|
|operação|registryOperation|Operação que foi alterado o nome da chave do registro e/ou valor. Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.|
|processId|Int32|Processo de identificação (PID) do processo que modificou a chave do registro (processo detalhes aparecerão na coleção alerta 'processos').|
|valueData|String|Dados de valor da chave do registro (ou seja alterado) atual (conteúdo).|
|valueName|String|Nome do valor da chave do registro (ou seja alterado) atual|
|valueType|registryValueType|[Tipo de valor da chave do registro](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

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