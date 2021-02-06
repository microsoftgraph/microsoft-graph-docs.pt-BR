---
title: Tipo de recurso applicationServicePrincipal
description: Uma combinação de um aplicativo e um servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: d69a9942e0ef14ddb866794b46a06c02d57dec62
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134754"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="906de-103">Tipo de recurso applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="906de-103">applicationServicePrincipal resource type</span></span>

<span data-ttu-id="906de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="906de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="906de-105">Quando uma instância de um aplicativo da galeria de aplicativos do Azure AD é adicionada, objetos [de](../resources/application.md) aplicativo e [servicePrincipal](../resources/serviceprincipal.md) são criados no diretório.</span><span class="sxs-lookup"><span data-stu-id="906de-105">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="906de-106">O **applicationServicePrincipal** representa a concatenação do **aplicativo e** do objeto **servicePrincipal.**</span><span class="sxs-lookup"><span data-stu-id="906de-106">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="906de-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="906de-107">Methods</span></span>

<span data-ttu-id="906de-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="906de-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="906de-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="906de-109">Properties</span></span>

| <span data-ttu-id="906de-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="906de-110">Property</span></span> | <span data-ttu-id="906de-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="906de-111">Type</span></span>        | <span data-ttu-id="906de-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="906de-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="906de-113">application</span><span class="sxs-lookup"><span data-stu-id="906de-113">application</span></span>|[<span data-ttu-id="906de-114">aplicativo</span><span class="sxs-lookup"><span data-stu-id="906de-114">application</span></span>](../resources/application.md)|<span data-ttu-id="906de-115">Representa um aplicativo registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="906de-115">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="906de-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="906de-116">servicePrincipal</span></span>|[<span data-ttu-id="906de-117">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="906de-117">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="906de-118">Representa uma instância de um aplicativo em um diretório.</span><span class="sxs-lookup"><span data-stu-id="906de-118">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="906de-119">Relações</span><span class="sxs-lookup"><span data-stu-id="906de-119">Relationships</span></span>

<span data-ttu-id="906de-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="906de-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="906de-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="906de-121">JSON representation</span></span>

<span data-ttu-id="906de-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="906de-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
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


