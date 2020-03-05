---
title: tipo de recurso accessPackageSubject
description: No Azure AD pretitulation Management, um assunto de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0f71b23e48c818747a2b70b52ec8b4baa53bf118
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508489"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="10e61-103">tipo de recurso accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="10e61-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="10e61-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="10e61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e61-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um pacote de acesso assunto é um usuário, uma entidade de serviço ou outra entidade que pode ser configurada para solicitar ou receber um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="10e61-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="10e61-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10e61-106">Properties</span></span>

| <span data-ttu-id="10e61-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10e61-107">Property</span></span>     | <span data-ttu-id="10e61-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="10e61-108">Type</span></span>        | <span data-ttu-id="10e61-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="10e61-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10e61-110">displayName</span><span class="sxs-lookup"><span data-stu-id="10e61-110">displayName</span></span>|<span data-ttu-id="10e61-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10e61-111">String</span></span>|<span data-ttu-id="10e61-112">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="10e61-112">The display name of the subject.</span></span>|
|<span data-ttu-id="10e61-113">email</span><span class="sxs-lookup"><span data-stu-id="10e61-113">email</span></span>|<span data-ttu-id="10e61-114">String</span><span class="sxs-lookup"><span data-stu-id="10e61-114">String</span></span>|<span data-ttu-id="10e61-115">O endereço de email do assunto.</span><span class="sxs-lookup"><span data-stu-id="10e61-115">The email address of the subject.</span></span>|
|<span data-ttu-id="10e61-116">id</span><span class="sxs-lookup"><span data-stu-id="10e61-116">id</span></span>|<span data-ttu-id="10e61-117">String</span><span class="sxs-lookup"><span data-stu-id="10e61-117">String</span></span>| <span data-ttu-id="10e61-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10e61-118">Read-only.</span></span>|
|<span data-ttu-id="10e61-119">objectId</span><span class="sxs-lookup"><span data-stu-id="10e61-119">objectId</span></span>|<span data-ttu-id="10e61-120">String</span><span class="sxs-lookup"><span data-stu-id="10e61-120">String</span></span>|<span data-ttu-id="10e61-121">A ID de objeto do assunto.</span><span class="sxs-lookup"><span data-stu-id="10e61-121">The object ID of the subject.</span></span>|
|<span data-ttu-id="10e61-122">principalName</span><span class="sxs-lookup"><span data-stu-id="10e61-122">principalName</span></span>|<span data-ttu-id="10e61-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10e61-123">String</span></span>|<span data-ttu-id="10e61-124">O nome da entidade de segurança, se for conhecido, do assunto.</span><span class="sxs-lookup"><span data-stu-id="10e61-124">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="10e61-125">type</span><span class="sxs-lookup"><span data-stu-id="10e61-125">type</span></span>|<span data-ttu-id="10e61-126">String</span><span class="sxs-lookup"><span data-stu-id="10e61-126">String</span></span>|<span data-ttu-id="10e61-127">O tipo de recurso do assunto.</span><span class="sxs-lookup"><span data-stu-id="10e61-127">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10e61-128">Relações</span><span class="sxs-lookup"><span data-stu-id="10e61-128">Relationships</span></span>

<span data-ttu-id="10e61-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10e61-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10e61-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10e61-130">JSON representation</span></span>

<span data-ttu-id="10e61-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10e61-131">The following is a JSON representation of the resource.</span></span>

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
