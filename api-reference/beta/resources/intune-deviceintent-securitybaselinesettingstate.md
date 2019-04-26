---
title: tipo de recurso securityBaselineSettingState
description: O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562276"
---
# <a name="securitybaselinesettingstate-resource-type"></a>tipo de recurso securityBaselineSettingState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityBaselineSettingStates](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|coleção [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Listar Propriedades e relações dos objetos [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .|
|[Obter securityBaselineSettingState](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Leia as propriedades e as relações do objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .|
|[Criar securityBaselineSettingState](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Criar um novo objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .|
|[Excluir securityBaselineSettingState](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|Nenhum|Exclui [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).|
|[Atualizar securityBaselineSettingState](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Atualiza as propriedades de um objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade|
|settingName|Cadeia de caracteres|O nome da configuração que está sendo relatado|
|estado|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|O estado de conformidade da configuração da linha de base de segurança. Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|settingCategoryId|String|A ID da categoria de configuração à qual essa configuração pertence|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "String (identifier)",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```



