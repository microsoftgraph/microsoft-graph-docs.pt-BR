---
title: tipo de recurso windowsKioskAzureADGroup
description: A classe usada para identificar um grupo do AzureAD para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c312f5fbefdf156bda98f8f82ce68c4e0d3213f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466790"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="6b99e-103">tipo de recurso windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="6b99e-103">windowsKioskAzureADGroup resource type</span></span>

<span data-ttu-id="6b99e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b99e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b99e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b99e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b99e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b99e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b99e-107">A classe usada para identificar um grupo do AzureAD para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="6b99e-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="6b99e-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="6b99e-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6b99e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b99e-109">Properties</span></span>
|<span data-ttu-id="6b99e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b99e-110">Property</span></span>|<span data-ttu-id="6b99e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b99e-111">Type</span></span>|<span data-ttu-id="6b99e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b99e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b99e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6b99e-113">displayName</span></span>|<span data-ttu-id="6b99e-114">String</span><span class="sxs-lookup"><span data-stu-id="6b99e-114">String</span></span>|<span data-ttu-id="6b99e-115">O nome de exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="6b99e-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="6b99e-116">groupId</span><span class="sxs-lookup"><span data-stu-id="6b99e-116">groupId</span></span>|<span data-ttu-id="6b99e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b99e-117">String</span></span>|<span data-ttu-id="6b99e-118">A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="6b99e-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b99e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6b99e-119">Relationships</span></span>
<span data-ttu-id="6b99e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b99e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b99e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b99e-121">JSON Representation</span></span>
<span data-ttu-id="6b99e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b99e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```



