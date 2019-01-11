---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0b9d7df95ce8ddb71439763eb02b205772e06300
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820318"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="953e8-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="953e8-103">appListItem resource type</span></span>

> <span data-ttu-id="953e8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="953e8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="953e8-105">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="953e8-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="953e8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="953e8-106">Properties</span></span>
|<span data-ttu-id="953e8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="953e8-107">Property</span></span>|<span data-ttu-id="953e8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="953e8-108">Type</span></span>|<span data-ttu-id="953e8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="953e8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="953e8-110">name</span><span class="sxs-lookup"><span data-stu-id="953e8-110">name</span></span>|<span data-ttu-id="953e8-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="953e8-111">String</span></span>|<span data-ttu-id="953e8-112">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="953e8-112">The application name</span></span>|
|<span data-ttu-id="953e8-113">distribuidor</span><span class="sxs-lookup"><span data-stu-id="953e8-113">publisher</span></span>|<span data-ttu-id="953e8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="953e8-114">String</span></span>|<span data-ttu-id="953e8-115">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="953e8-115">The publisher of the application</span></span>|
|<span data-ttu-id="953e8-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="953e8-116">appStoreUrl</span></span>|<span data-ttu-id="953e8-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="953e8-117">String</span></span>|<span data-ttu-id="953e8-118">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="953e8-118">The Store URL of the application</span></span>|
|<span data-ttu-id="953e8-119">appId</span><span class="sxs-lookup"><span data-stu-id="953e8-119">appId</span></span>|<span data-ttu-id="953e8-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="953e8-120">String</span></span>|<span data-ttu-id="953e8-121">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="953e8-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="953e8-122">Relações</span><span class="sxs-lookup"><span data-stu-id="953e8-122">Relationships</span></span>
<span data-ttu-id="953e8-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="953e8-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="953e8-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="953e8-124">JSON Representation</span></span>
<span data-ttu-id="953e8-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="953e8-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



