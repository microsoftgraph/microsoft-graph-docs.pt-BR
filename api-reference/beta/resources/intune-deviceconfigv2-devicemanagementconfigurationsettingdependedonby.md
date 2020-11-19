---
title: tipo de recurso deviceManagementConfigurationSettingDependedOnBy
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3d9b6bde7217460867ab7e9b77853fcb366e38c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241142"
---
# <a name="devicemanagementconfigurationsettingdependedonby-resource-type"></a><span data-ttu-id="a5484-103">tipo de recurso deviceManagementConfigurationSettingDependedOnBy</span><span class="sxs-lookup"><span data-stu-id="a5484-103">deviceManagementConfigurationSettingDependedOnBy resource type</span></span>

<span data-ttu-id="a5484-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5484-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5484-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5484-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5484-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5484-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5484-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5484-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a5484-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5484-108">Properties</span></span>
|<span data-ttu-id="a5484-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5484-109">Property</span></span>|<span data-ttu-id="a5484-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5484-110">Type</span></span>|<span data-ttu-id="a5484-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5484-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5484-112">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="a5484-112">dependedOnBy</span></span>|<span data-ttu-id="a5484-113">String</span><span class="sxs-lookup"><span data-stu-id="a5484-113">String</span></span>|<span data-ttu-id="a5484-114">Identificador da configuração filha dependente da configuração atual</span><span class="sxs-lookup"><span data-stu-id="a5484-114">Identifier of child setting that is dependent on the current setting</span></span>|
|<span data-ttu-id="a5484-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="a5484-115">required</span></span>|<span data-ttu-id="a5484-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5484-116">Boolean</span></span>|<span data-ttu-id="a5484-117">O valor que determina se a configuração filha é necessária com base na seleção da configuração pai</span><span class="sxs-lookup"><span data-stu-id="a5484-117">Value that determines if the child setting is required based on the parent setting's selection</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5484-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a5484-118">Relationships</span></span>
<span data-ttu-id="a5484-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5484-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5484-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5484-120">JSON Representation</span></span>
<span data-ttu-id="a5484-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5484-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
  "dependedOnBy": "String",
  "required": true
}
```




