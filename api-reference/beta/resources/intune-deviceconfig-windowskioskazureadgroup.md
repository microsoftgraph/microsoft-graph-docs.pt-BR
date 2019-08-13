---
title: tipo de recurso windowsKioskAzureADGroup
description: A classe usada para identificar um grupo do AzureAD para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00cd2f43fb09df03dfe2f5ee1810871dc2b77fb2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370939"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="78b57-103">tipo de recurso windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="78b57-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="78b57-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78b57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78b57-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78b57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78b57-106">A classe usada para identificar um grupo do AzureAD para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="78b57-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="78b57-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="78b57-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78b57-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78b57-108">Properties</span></span>
|<span data-ttu-id="78b57-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78b57-109">Property</span></span>|<span data-ttu-id="78b57-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="78b57-110">Type</span></span>|<span data-ttu-id="78b57-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="78b57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78b57-112">displayName</span><span class="sxs-lookup"><span data-stu-id="78b57-112">displayName</span></span>|<span data-ttu-id="78b57-113">String</span><span class="sxs-lookup"><span data-stu-id="78b57-113">String</span></span>|<span data-ttu-id="78b57-114">O nome de exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="78b57-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="78b57-115">groupId</span><span class="sxs-lookup"><span data-stu-id="78b57-115">groupId</span></span>|<span data-ttu-id="78b57-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78b57-116">String</span></span>|<span data-ttu-id="78b57-117">A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="78b57-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="78b57-118">Relações</span><span class="sxs-lookup"><span data-stu-id="78b57-118">Relationships</span></span>
<span data-ttu-id="78b57-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78b57-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78b57-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78b57-120">JSON Representation</span></span>
<span data-ttu-id="78b57-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78b57-121">Here is a JSON representation of the resource.</span></span>
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



