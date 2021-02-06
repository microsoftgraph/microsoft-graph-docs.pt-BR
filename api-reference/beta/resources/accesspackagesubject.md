---
title: Tipo de recurso accessPackageSubject
description: No gerenciamento de direitos do Azure AD, um assunto de uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4969afac14f7eeb24d2901946d5e5961258c8b7b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133573"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="aba2b-103">Tipo de recurso accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="aba2b-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="aba2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aba2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aba2b-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um assunto do pacote de acesso é um usuário, entidade de serviço ou outra entidade que pode ser configurada para solicitar ou ser atribuído a um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="aba2b-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="aba2b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aba2b-106">Properties</span></span>

| <span data-ttu-id="aba2b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aba2b-107">Property</span></span>     | <span data-ttu-id="aba2b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="aba2b-108">Type</span></span>        | <span data-ttu-id="aba2b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aba2b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aba2b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="aba2b-110">displayName</span></span>|<span data-ttu-id="aba2b-111">String</span><span class="sxs-lookup"><span data-stu-id="aba2b-111">String</span></span>|<span data-ttu-id="aba2b-112">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="aba2b-112">The display name of the subject.</span></span>|
|<span data-ttu-id="aba2b-113">email</span><span class="sxs-lookup"><span data-stu-id="aba2b-113">email</span></span>|<span data-ttu-id="aba2b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aba2b-114">String</span></span>|<span data-ttu-id="aba2b-115">O endereço de email do assunto.</span><span class="sxs-lookup"><span data-stu-id="aba2b-115">The email address of the subject.</span></span>|
|<span data-ttu-id="aba2b-116">id</span><span class="sxs-lookup"><span data-stu-id="aba2b-116">id</span></span>|<span data-ttu-id="aba2b-117">String</span><span class="sxs-lookup"><span data-stu-id="aba2b-117">String</span></span>| <span data-ttu-id="aba2b-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aba2b-118">Read-only.</span></span>|
|<span data-ttu-id="aba2b-119">objectId</span><span class="sxs-lookup"><span data-stu-id="aba2b-119">objectId</span></span>|<span data-ttu-id="aba2b-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aba2b-120">String</span></span>|<span data-ttu-id="aba2b-121">A ID do objeto do assunto.</span><span class="sxs-lookup"><span data-stu-id="aba2b-121">The object ID of the subject.</span></span>|
|<span data-ttu-id="aba2b-122">principalName</span><span class="sxs-lookup"><span data-stu-id="aba2b-122">principalName</span></span>|<span data-ttu-id="aba2b-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aba2b-123">String</span></span>|<span data-ttu-id="aba2b-124">O nome principal, se conhecido, do assunto.</span><span class="sxs-lookup"><span data-stu-id="aba2b-124">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="aba2b-125">type</span><span class="sxs-lookup"><span data-stu-id="aba2b-125">type</span></span>|<span data-ttu-id="aba2b-126">String</span><span class="sxs-lookup"><span data-stu-id="aba2b-126">String</span></span>|<span data-ttu-id="aba2b-127">O tipo de recurso do assunto.</span><span class="sxs-lookup"><span data-stu-id="aba2b-127">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aba2b-128">Relações</span><span class="sxs-lookup"><span data-stu-id="aba2b-128">Relationships</span></span>

<span data-ttu-id="aba2b-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aba2b-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aba2b-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aba2b-130">JSON representation</span></span>

<span data-ttu-id="aba2b-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aba2b-131">The following is a JSON representation of the resource.</span></span>

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


