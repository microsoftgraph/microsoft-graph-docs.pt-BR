---
title: tipo de recurso deviceManagementSettingRequiredConstraint
description: Restrição que impõe uma determinada configuração necessária que não é nula/indefinida/sequência vazia/não configurada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 732e266bcc111c0e07a110a6abc7171798d7d885
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267932"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="971ee-103">tipo de recurso deviceManagementSettingRequiredConstraint</span><span class="sxs-lookup"><span data-stu-id="971ee-103">deviceManagementSettingRequiredConstraint resource type</span></span>

<span data-ttu-id="971ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="971ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="971ee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="971ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="971ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="971ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="971ee-107">Restrição que impõe uma determinada configuração necessária que não é nula/indefinida/sequência vazia/não configurada</span><span class="sxs-lookup"><span data-stu-id="971ee-107">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="971ee-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="971ee-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="971ee-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="971ee-109">Properties</span></span>
|<span data-ttu-id="971ee-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="971ee-110">Property</span></span>|<span data-ttu-id="971ee-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="971ee-111">Type</span></span>|<span data-ttu-id="971ee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="971ee-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="971ee-113">Não configuravalue</span><span class="sxs-lookup"><span data-stu-id="971ee-113">notConfiguredValue</span></span>|<span data-ttu-id="971ee-114">String</span><span class="sxs-lookup"><span data-stu-id="971ee-114">String</span></span>|<span data-ttu-id="971ee-115">Lista de valores que significa não configurado para a configuração</span><span class="sxs-lookup"><span data-stu-id="971ee-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="971ee-116">Relações</span><span class="sxs-lookup"><span data-stu-id="971ee-116">Relationships</span></span>
<span data-ttu-id="971ee-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="971ee-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="971ee-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="971ee-118">JSON Representation</span></span>
<span data-ttu-id="971ee-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="971ee-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRequiredConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRequiredConstraint",
  "notConfiguredValue": "String"
}
```




