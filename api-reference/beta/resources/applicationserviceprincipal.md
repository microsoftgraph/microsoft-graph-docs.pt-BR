---
title: tipo de recurso applicationServicePrincipal
description: Uma combinação de um aplicativo e um servicePrincipalName.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9a7cc33e05c28e5552815778e86e5b1b9e7aaf06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508279"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="8681d-103">tipo de recurso applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="8681d-103">applicationServicePrincipal resource type</span></span>

<span data-ttu-id="8681d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8681d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8681d-105">Quando uma instância de um aplicativo da Galeria de aplicativos do Azure AD é adicionada, os objetos [Application](../resources/application.md) e [UserPrincipal](../resources/serviceprincipal.md) são criados no diretório.</span><span class="sxs-lookup"><span data-stu-id="8681d-105">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="8681d-106">O **applicationServicePrincipal** representa a concatenação do **aplicativo** e do objeto **servicePrincipalName** .</span><span class="sxs-lookup"><span data-stu-id="8681d-106">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="8681d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8681d-107">Methods</span></span>

<span data-ttu-id="8681d-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8681d-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="8681d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8681d-109">Properties</span></span>

| <span data-ttu-id="8681d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8681d-110">Property</span></span> | <span data-ttu-id="8681d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8681d-111">Type</span></span>        | <span data-ttu-id="8681d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8681d-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8681d-113">application</span><span class="sxs-lookup"><span data-stu-id="8681d-113">application</span></span>|[<span data-ttu-id="8681d-114">application</span><span class="sxs-lookup"><span data-stu-id="8681d-114">application</span></span>](../resources/application.md)|<span data-ttu-id="8681d-115">Representa um aplicativo registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8681d-115">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="8681d-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="8681d-116">servicePrincipal</span></span>|[<span data-ttu-id="8681d-117">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="8681d-117">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="8681d-118">Representa uma instância de um aplicativo em um diretório.</span><span class="sxs-lookup"><span data-stu-id="8681d-118">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8681d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="8681d-119">Relationships</span></span>

<span data-ttu-id="8681d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8681d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8681d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8681d-121">JSON representation</span></span>

<span data-ttu-id="8681d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8681d-122">The following is a JSON representation of the resource.</span></span>

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
