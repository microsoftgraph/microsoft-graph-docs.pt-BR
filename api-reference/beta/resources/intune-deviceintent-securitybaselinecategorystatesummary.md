---
title: Tipo de recurso securityBaselineCategoryStateSummary
description: O resumo do estado de conformidade da linha de base de segurança por categoria para a linha de base de segurança da conta.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc0bb04e7545ade025b3659a921ccb34237a0290
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801469"
---
# <a name="securitybaselinecategorystatesummary-resource-type"></a>Tipo de recurso securityBaselineCategoryStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo do estado de conformidade da linha de base de segurança por categoria para a linha de base de segurança da conta.


Herda de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityBaselineCategoryStateSummaries](../api/intune-deviceintent-securitybaselinecategorystatesummary-list.md)|[coleção securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Listar propriedades e relações dos [objetos securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|
|[Obter securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-get.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Leia propriedades e relações do [objeto securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|
|[Criar securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-create.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Crie um novo [objeto securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|
|[Excluir securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-delete.md)|Nenhum(a)|Exclui um [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).|
|[Atualizar securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-update.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Atualize as propriedades de [um objeto securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade. Herdado [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|secureCount|Int32|Número de dispositivos seguros Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notSecureCount|Int32|Número de dispositivos não seguros Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|unknownCount|Int32|Número de dispositivos desconhecidos Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|errorCount|Int32|Número de dispositivos de erro Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|conflictCount|Int32|Número de dispositivos de conflito Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notApplicableCount|Int32|Número de dispositivos não aplicáveis Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|displayName|Cadeia de caracteres|O nome da categoria|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineCategoryStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024,
  "displayName": "String"
}
```



