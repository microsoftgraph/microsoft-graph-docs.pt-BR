---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb861ad99aa3d8d73fd096af33377722c74feace
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527088"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="eb033-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="eb033-103">appListItem resource type</span></span>

<span data-ttu-id="eb033-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb033-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb033-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb033-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb033-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb033-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb033-107">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="eb033-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="eb033-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb033-108">Properties</span></span>
|<span data-ttu-id="eb033-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb033-109">Property</span></span>|<span data-ttu-id="eb033-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb033-110">Type</span></span>|<span data-ttu-id="eb033-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb033-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb033-112">nome</span><span class="sxs-lookup"><span data-stu-id="eb033-112">name</span></span>|<span data-ttu-id="eb033-113">String</span><span class="sxs-lookup"><span data-stu-id="eb033-113">String</span></span>|<span data-ttu-id="eb033-114">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb033-114">The application name</span></span>|
|<span data-ttu-id="eb033-115">distribuidor</span><span class="sxs-lookup"><span data-stu-id="eb033-115">publisher</span></span>|<span data-ttu-id="eb033-116">String</span><span class="sxs-lookup"><span data-stu-id="eb033-116">String</span></span>|<span data-ttu-id="eb033-117">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb033-117">The publisher of the application</span></span>|
|<span data-ttu-id="eb033-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="eb033-118">appStoreUrl</span></span>|<span data-ttu-id="eb033-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb033-119">String</span></span>|<span data-ttu-id="eb033-120">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb033-120">The Store URL of the application</span></span>|
|<span data-ttu-id="eb033-121">appId</span><span class="sxs-lookup"><span data-stu-id="eb033-121">appId</span></span>|<span data-ttu-id="eb033-122">String</span><span class="sxs-lookup"><span data-stu-id="eb033-122">String</span></span>|<span data-ttu-id="eb033-123">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb033-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb033-124">Relações</span><span class="sxs-lookup"><span data-stu-id="eb033-124">Relationships</span></span>
<span data-ttu-id="eb033-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb033-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb033-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb033-126">JSON Representation</span></span>
<span data-ttu-id="eb033-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb033-127">Here is a JSON representation of the resource.</span></span>
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



