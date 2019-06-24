---
title: tipo de recurso applicationServicePrincipal
description: Uma combinação de um aplicativo e um servicePrincipalName.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3a6d0d1017f89587f1f826c4225eefc51dc5edb
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147888"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="19c47-103">tipo de recurso applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="19c47-103">applicationServicePrincipal resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19c47-104">Quando uma instância de um aplicativo da Galeria de aplicativos do Azure AD é adicionada, os objetos [Application](../resources/application.md) e UserPrincipal são criados no diretório. [](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="19c47-104">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="19c47-105">O **applicationServicePrincipal** representa a concatenação do **aplicativo** e do objeto **servicePrincipalName** .</span><span class="sxs-lookup"><span data-stu-id="19c47-105">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="19c47-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="19c47-106">Methods</span></span>

<span data-ttu-id="19c47-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19c47-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="19c47-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19c47-108">Properties</span></span>

| <span data-ttu-id="19c47-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19c47-109">Property</span></span> | <span data-ttu-id="19c47-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="19c47-110">Type</span></span>        | <span data-ttu-id="19c47-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="19c47-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19c47-112">application</span><span class="sxs-lookup"><span data-stu-id="19c47-112">application</span></span>|[<span data-ttu-id="19c47-113">application</span><span class="sxs-lookup"><span data-stu-id="19c47-113">application</span></span>](../resources/application.md)|<span data-ttu-id="19c47-114">Representa um aplicativo registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="19c47-114">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="19c47-115">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="19c47-115">servicePrincipal</span></span>|[<span data-ttu-id="19c47-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="19c47-116">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="19c47-117">Representa uma instância de um aplicativo em um diretório.</span><span class="sxs-lookup"><span data-stu-id="19c47-117">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19c47-118">Relações</span><span class="sxs-lookup"><span data-stu-id="19c47-118">Relationships</span></span>

<span data-ttu-id="19c47-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19c47-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19c47-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19c47-120">JSON representation</span></span>

<span data-ttu-id="19c47-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19c47-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
