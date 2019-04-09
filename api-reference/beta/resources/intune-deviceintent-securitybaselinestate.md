---
title: tipo de recurso securityBaselineState
description: Estado da linha de base de segurança para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c81a3d351c7c1e854c26e05e32f8426ffdc0631
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524558"
---
# <a name="securitybaselinestate-resource-type"></a>tipo de recurso securityBaselineState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado da linha de base de segurança para um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityBaselineStates](../api/intune-deviceintent-securitybaselinestate-list.md)|coleção [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|Listar Propriedades e relações dos objetos [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .|
|[Obter securityBaselineState](../api/intune-deviceintent-securitybaselinestate-get.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|Leia as propriedades e as relações do objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .|
|[Criar securityBaselineState](../api/intune-deviceintent-securitybaselinestate-create.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|Criar um novo objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .|
|[Excluir securityBaselineState](../api/intune-deviceintent-securitybaselinestate-delete.md)|Nenhum|Exclui [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).|
|[Atualizar securityBaselineState](../api/intune-deviceintent-securitybaselinestate-update.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|Atualiza as propriedades de um objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|securityBaselineTemplateId|Cadeia de Caracteres|A ID do modelo de linha de base de segurança|
|displayName|String|O nome de exibição da linha de base de segurança|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settingStates|coleção [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|O estado da linha de base de segurança para configurações diferentes de um dispositivo|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "String (identifier)",
  "securityBaselineTemplateId": "String",
  "displayName": "String"
}
```



