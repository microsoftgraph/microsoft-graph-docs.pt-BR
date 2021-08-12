---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6876d956fa989355ad7ea6ca28171c8c0a49b7661e987d3de5aece0972130403
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146493"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-companyterms-devicemanagement-get.md)|[deviceManagement](../resources/intune-companyterms-devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-companyterms-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-companyterms-devicemanagement-update.md)|[deviceManagement](../resources/intune-companyterms-devicemanagement.md)|Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-companyterms-devicemanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|termsAndConditions|Conjunto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Os termos e condições associados ao gerenciamento do dispositivo da empresa.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




