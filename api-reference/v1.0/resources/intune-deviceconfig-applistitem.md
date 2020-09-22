---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a53da1a1e50b0537a20d763b49957369a28556ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051127"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="5b60b-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="5b60b-103">appListItem resource type</span></span>

<span data-ttu-id="5b60b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b60b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b60b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b60b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b60b-106">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="5b60b-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="5b60b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b60b-107">Properties</span></span>
|<span data-ttu-id="5b60b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b60b-108">Property</span></span>|<span data-ttu-id="5b60b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b60b-109">Type</span></span>|<span data-ttu-id="5b60b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b60b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b60b-111">nome</span><span class="sxs-lookup"><span data-stu-id="5b60b-111">name</span></span>|<span data-ttu-id="5b60b-112">String</span><span class="sxs-lookup"><span data-stu-id="5b60b-112">String</span></span>|<span data-ttu-id="5b60b-113">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b60b-113">The application name</span></span>|
|<span data-ttu-id="5b60b-114">distribuidor</span><span class="sxs-lookup"><span data-stu-id="5b60b-114">publisher</span></span>|<span data-ttu-id="5b60b-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b60b-115">String</span></span>|<span data-ttu-id="5b60b-116">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b60b-116">The publisher of the application</span></span>|
|<span data-ttu-id="5b60b-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5b60b-117">appStoreUrl</span></span>|<span data-ttu-id="5b60b-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b60b-118">String</span></span>|<span data-ttu-id="5b60b-119">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b60b-119">The Store URL of the application</span></span>|
|<span data-ttu-id="5b60b-120">appId</span><span class="sxs-lookup"><span data-stu-id="5b60b-120">appId</span></span>|<span data-ttu-id="5b60b-121">String</span><span class="sxs-lookup"><span data-stu-id="5b60b-121">String</span></span>|<span data-ttu-id="5b60b-122">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b60b-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b60b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="5b60b-123">Relationships</span></span>
<span data-ttu-id="5b60b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b60b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b60b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b60b-125">JSON Representation</span></span>
<span data-ttu-id="5b60b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b60b-126">Here is a JSON representation of the resource.</span></span>
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









