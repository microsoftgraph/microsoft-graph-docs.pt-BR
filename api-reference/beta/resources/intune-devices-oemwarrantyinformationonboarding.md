---
title: Tipo de recurso oemWarrantyInformationOnboarding
description: Entidade de status da garantia para um determinado OEM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90cfa2ba539f50fe7c550fe6b22cad7d88c7e265
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292300"
---
# <a name="oemwarrantyinformationonboarding-resource-type"></a>Tipo de recurso oemWarrantyInformationOnboarding

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade de status da garantia para um determinado OEM

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar oemWarrantyInformationOnboardings](../api/intune-devices-oemwarrantyinformationonboarding-list.md)|[Coleção oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|Listar propriedades e relações dos [objetos oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .|
|[Obter oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-get.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|Leia propriedades e relações do [objeto oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .|
|[Criar oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-create.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|Crie um novo [objeto oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .|
|[Excluir oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-delete.md)|Nenhuma|Exclui um [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md).|
|[Atualizar oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-update.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|Atualize as propriedades de [um objeto oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) .|
|[habilitar ação](../api/intune-devices-oemwarrantyinformationonboarding-enable.md)|Nenhuma|Ainda não documentado|
|[desabilitar ação](../api/intune-devices-oemwarrantyinformationonboarding-disable.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o status da Garantia OEM. Essa propriedade é somente leitura.|
|oemName|Cadeia de caracteres|Nome OEM. Essa propriedade é somente leitura.|
|enabled|Boolean|Especifica se a consulta de garantia está habilitada para determinado OEM. Essa propriedade é somente leitura.|
|disponível|Booliano|Especifica se a API de garantia está disponível. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.oemWarrantyInformationOnboarding"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oemWarrantyInformationOnboarding",
  "id": "String (identifier)",
  "oemName": "String",
  "enabled": true,
  "available": true
}
```




