---
title: tipo de recurso accessPackageSubject
description: No Azure AD pretitulation Management, um assunto de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8b967e2ba2d678d9648b09eae4aeb3dca760c52
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994341"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="ac726-103">tipo de recurso accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="ac726-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="ac726-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac726-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac726-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um pacote de acesso assunto é um usuário, uma entidade de serviço ou outra entidade que pode ser configurada para solicitar ou receber um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="ac726-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="ac726-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac726-106">Properties</span></span>

| <span data-ttu-id="ac726-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac726-107">Property</span></span>     | <span data-ttu-id="ac726-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac726-108">Type</span></span>        | <span data-ttu-id="ac726-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac726-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac726-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ac726-110">displayName</span></span>|<span data-ttu-id="ac726-111">String</span><span class="sxs-lookup"><span data-stu-id="ac726-111">String</span></span>|<span data-ttu-id="ac726-112">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="ac726-112">The display name of the subject.</span></span>|
|<span data-ttu-id="ac726-113">email</span><span class="sxs-lookup"><span data-stu-id="ac726-113">email</span></span>|<span data-ttu-id="ac726-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac726-114">String</span></span>|<span data-ttu-id="ac726-115">O endereço de email do assunto.</span><span class="sxs-lookup"><span data-stu-id="ac726-115">The email address of the subject.</span></span>|
|<span data-ttu-id="ac726-116">id</span><span class="sxs-lookup"><span data-stu-id="ac726-116">id</span></span>|<span data-ttu-id="ac726-117">String</span><span class="sxs-lookup"><span data-stu-id="ac726-117">String</span></span>| <span data-ttu-id="ac726-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac726-118">Read-only.</span></span>|
|<span data-ttu-id="ac726-119">objectId</span><span class="sxs-lookup"><span data-stu-id="ac726-119">objectId</span></span>|<span data-ttu-id="ac726-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac726-120">String</span></span>|<span data-ttu-id="ac726-121">A ID de objeto do assunto.</span><span class="sxs-lookup"><span data-stu-id="ac726-121">The object ID of the subject.</span></span>|
|<span data-ttu-id="ac726-122">principalName</span><span class="sxs-lookup"><span data-stu-id="ac726-122">principalName</span></span>|<span data-ttu-id="ac726-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac726-123">String</span></span>|<span data-ttu-id="ac726-124">O nome da entidade de segurança, se for conhecido, do assunto.</span><span class="sxs-lookup"><span data-stu-id="ac726-124">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="ac726-125">tipo</span><span class="sxs-lookup"><span data-stu-id="ac726-125">type</span></span>|<span data-ttu-id="ac726-126">String</span><span class="sxs-lookup"><span data-stu-id="ac726-126">String</span></span>|<span data-ttu-id="ac726-127">O tipo de recurso do assunto.</span><span class="sxs-lookup"><span data-stu-id="ac726-127">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac726-128">Relações</span><span class="sxs-lookup"><span data-stu-id="ac726-128">Relationships</span></span>

<span data-ttu-id="ac726-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac726-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac726-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac726-130">JSON representation</span></span>

<span data-ttu-id="ac726-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac726-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "Administrator",
  "email": "admin@contoso.com",
  "id": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
  "objectId": "cc754ed5-f598-45c0-aaf0-fc2f2eb1838f",
  "principalName": "admin@domain.contoso.com",
  "type": "User"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageSubject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


