---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9571b622fc098f384f7c3a6c62b1d1e10d89f663
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405412"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="6f6ee-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="6f6ee-103">appListItem resource type</span></span>

> <span data-ttu-id="6f6ee-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f6ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f6ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f6ee-107">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="6f6ee-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="6f6ee-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f6ee-108">Properties</span></span>
|<span data-ttu-id="6f6ee-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f6ee-109">Property</span></span>|<span data-ttu-id="6f6ee-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f6ee-110">Type</span></span>|<span data-ttu-id="6f6ee-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f6ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f6ee-112">name</span><span class="sxs-lookup"><span data-stu-id="6f6ee-112">name</span></span>|<span data-ttu-id="6f6ee-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f6ee-113">String</span></span>|<span data-ttu-id="6f6ee-114">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f6ee-114">The application name</span></span>|
|<span data-ttu-id="6f6ee-115">distribuidor</span><span class="sxs-lookup"><span data-stu-id="6f6ee-115">publisher</span></span>|<span data-ttu-id="6f6ee-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f6ee-116">String</span></span>|<span data-ttu-id="6f6ee-117">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f6ee-117">The publisher of the application</span></span>|
|<span data-ttu-id="6f6ee-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6f6ee-118">appStoreUrl</span></span>|<span data-ttu-id="6f6ee-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f6ee-119">String</span></span>|<span data-ttu-id="6f6ee-120">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f6ee-120">The Store URL of the application</span></span>|
|<span data-ttu-id="6f6ee-121">appId</span><span class="sxs-lookup"><span data-stu-id="6f6ee-121">appId</span></span>|<span data-ttu-id="6f6ee-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f6ee-122">String</span></span>|<span data-ttu-id="6f6ee-123">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f6ee-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f6ee-124">Relações</span><span class="sxs-lookup"><span data-stu-id="6f6ee-124">Relationships</span></span>
<span data-ttu-id="6f6ee-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f6ee-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f6ee-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f6ee-126">JSON Representation</span></span>
<span data-ttu-id="6f6ee-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-127">Here is a JSON representation of the resource.</span></span>
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




