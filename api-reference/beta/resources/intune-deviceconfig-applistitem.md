---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d29fca9155ac14c7b8ebf9ad862bda3bed874353
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947712"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="09d44-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="09d44-103">appListItem resource type</span></span>

> <span data-ttu-id="09d44-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09d44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09d44-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09d44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09d44-106">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="09d44-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="09d44-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09d44-107">Properties</span></span>
|<span data-ttu-id="09d44-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09d44-108">Property</span></span>|<span data-ttu-id="09d44-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="09d44-109">Type</span></span>|<span data-ttu-id="09d44-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d44-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09d44-111">nome</span><span class="sxs-lookup"><span data-stu-id="09d44-111">name</span></span>|<span data-ttu-id="09d44-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09d44-112">String</span></span>|<span data-ttu-id="09d44-113">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="09d44-113">The application name</span></span>|
|<span data-ttu-id="09d44-114">distribuidor</span><span class="sxs-lookup"><span data-stu-id="09d44-114">publisher</span></span>|<span data-ttu-id="09d44-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09d44-115">String</span></span>|<span data-ttu-id="09d44-116">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="09d44-116">The publisher of the application</span></span>|
|<span data-ttu-id="09d44-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="09d44-117">appStoreUrl</span></span>|<span data-ttu-id="09d44-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09d44-118">String</span></span>|<span data-ttu-id="09d44-119">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="09d44-119">The Store URL of the application</span></span>|
|<span data-ttu-id="09d44-120">appId</span><span class="sxs-lookup"><span data-stu-id="09d44-120">appId</span></span>|<span data-ttu-id="09d44-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09d44-121">String</span></span>|<span data-ttu-id="09d44-122">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="09d44-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="09d44-123">Relações</span><span class="sxs-lookup"><span data-stu-id="09d44-123">Relationships</span></span>
<span data-ttu-id="09d44-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09d44-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09d44-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09d44-125">JSON Representation</span></span>
<span data-ttu-id="09d44-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09d44-126">Here is a JSON representation of the resource.</span></span>
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




