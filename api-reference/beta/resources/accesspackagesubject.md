---
title: tipo de recurso accessPackageSubject
description: No Azure AD pretitulation Management, um assunto de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0b37d91ad5669a0a87cef91893babf392f2f309b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939401"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="e967e-103">tipo de recurso accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="e967e-103">accessPackageSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e967e-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um pacote de acesso assunto é um usuário, uma entidade de serviço ou outra entidade que pode ser configurada para solicitar ou receber um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="e967e-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="e967e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e967e-105">Properties</span></span>

| <span data-ttu-id="e967e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e967e-106">Property</span></span>     | <span data-ttu-id="e967e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e967e-107">Type</span></span>        | <span data-ttu-id="e967e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e967e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e967e-109">displayName</span><span class="sxs-lookup"><span data-stu-id="e967e-109">displayName</span></span>|<span data-ttu-id="e967e-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e967e-110">String</span></span>|<span data-ttu-id="e967e-111">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="e967e-111">The display name of the subject.</span></span>|
|<span data-ttu-id="e967e-112">email</span><span class="sxs-lookup"><span data-stu-id="e967e-112">email</span></span>|<span data-ttu-id="e967e-113">String</span><span class="sxs-lookup"><span data-stu-id="e967e-113">String</span></span>|<span data-ttu-id="e967e-114">O endereço de email do assunto.</span><span class="sxs-lookup"><span data-stu-id="e967e-114">The email address of the subject.</span></span>|
|<span data-ttu-id="e967e-115">id</span><span class="sxs-lookup"><span data-stu-id="e967e-115">id</span></span>|<span data-ttu-id="e967e-116">String</span><span class="sxs-lookup"><span data-stu-id="e967e-116">String</span></span>| <span data-ttu-id="e967e-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e967e-117">Read-only.</span></span>|
|<span data-ttu-id="e967e-118">objectId</span><span class="sxs-lookup"><span data-stu-id="e967e-118">objectId</span></span>|<span data-ttu-id="e967e-119">String</span><span class="sxs-lookup"><span data-stu-id="e967e-119">String</span></span>|<span data-ttu-id="e967e-120">A ID de objeto do assunto.</span><span class="sxs-lookup"><span data-stu-id="e967e-120">The object ID of the subject.</span></span>|
|<span data-ttu-id="e967e-121">principalName</span><span class="sxs-lookup"><span data-stu-id="e967e-121">principalName</span></span>|<span data-ttu-id="e967e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e967e-122">String</span></span>|<span data-ttu-id="e967e-123">O nome da entidade de segurança, se for conhecido, do assunto.</span><span class="sxs-lookup"><span data-stu-id="e967e-123">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="e967e-124">type</span><span class="sxs-lookup"><span data-stu-id="e967e-124">type</span></span>|<span data-ttu-id="e967e-125">String</span><span class="sxs-lookup"><span data-stu-id="e967e-125">String</span></span>|<span data-ttu-id="e967e-126">O tipo de recurso do assunto.</span><span class="sxs-lookup"><span data-stu-id="e967e-126">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e967e-127">Relações</span><span class="sxs-lookup"><span data-stu-id="e967e-127">Relationships</span></span>

<span data-ttu-id="e967e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e967e-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e967e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e967e-129">JSON representation</span></span>

<span data-ttu-id="e967e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e967e-130">The following is a JSON representation of the resource.</span></span>

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
