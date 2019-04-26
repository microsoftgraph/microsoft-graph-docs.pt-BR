---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f452de7d002368c204cb57cc352ac9f9658609a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549556"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="f99aa-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="f99aa-103">appListItem resource type</span></span>

> <span data-ttu-id="f99aa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f99aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f99aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f99aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f99aa-106">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="f99aa-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="f99aa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f99aa-107">Properties</span></span>
|<span data-ttu-id="f99aa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f99aa-108">Property</span></span>|<span data-ttu-id="f99aa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f99aa-109">Type</span></span>|<span data-ttu-id="f99aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f99aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f99aa-111">name</span><span class="sxs-lookup"><span data-stu-id="f99aa-111">name</span></span>|<span data-ttu-id="f99aa-112">String</span><span class="sxs-lookup"><span data-stu-id="f99aa-112">String</span></span>|<span data-ttu-id="f99aa-113">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f99aa-113">The application name</span></span>|
|<span data-ttu-id="f99aa-114">distribuidor</span><span class="sxs-lookup"><span data-stu-id="f99aa-114">publisher</span></span>|<span data-ttu-id="f99aa-115">String</span><span class="sxs-lookup"><span data-stu-id="f99aa-115">String</span></span>|<span data-ttu-id="f99aa-116">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f99aa-116">The publisher of the application</span></span>|
|<span data-ttu-id="f99aa-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f99aa-117">appStoreUrl</span></span>|<span data-ttu-id="f99aa-118">String</span><span class="sxs-lookup"><span data-stu-id="f99aa-118">String</span></span>|<span data-ttu-id="f99aa-119">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f99aa-119">The Store URL of the application</span></span>|
|<span data-ttu-id="f99aa-120">appId</span><span class="sxs-lookup"><span data-stu-id="f99aa-120">appId</span></span>|<span data-ttu-id="f99aa-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f99aa-121">String</span></span>|<span data-ttu-id="f99aa-122">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f99aa-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f99aa-123">Relações</span><span class="sxs-lookup"><span data-stu-id="f99aa-123">Relationships</span></span>
<span data-ttu-id="f99aa-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f99aa-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f99aa-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f99aa-125">JSON Representation</span></span>
<span data-ttu-id="f99aa-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f99aa-126">Here is a JSON representation of the resource.</span></span>
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





