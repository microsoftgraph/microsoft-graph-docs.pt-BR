---
title: Tipo de recurso accessPackageSubject
description: No gerenciamento de direitos do Azure AD, um assunto de uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0adfca021ec463029a4b35c047ac85f8ce52921b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467054"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="d57f0-103">Tipo de recurso accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="d57f0-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="d57f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d57f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d57f0-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um assunto do pacote de acesso é um usuário, entidade de serviço ou outra entidade que pode ser configurada para solicitar ou ter um pacote de acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="d57f0-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>  <span data-ttu-id="d57f0-106">Ele pode representar um solicitante de uma organização conectada que ainda não está no locatário.</span><span class="sxs-lookup"><span data-stu-id="d57f0-106">It may represent a requestor from a connected organization who is not yet in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="d57f0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d57f0-107">Properties</span></span>

| <span data-ttu-id="d57f0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d57f0-108">Property</span></span>     | <span data-ttu-id="d57f0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d57f0-109">Type</span></span>        | <span data-ttu-id="d57f0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d57f0-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d57f0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d57f0-111">displayName</span></span>|<span data-ttu-id="d57f0-112">String</span><span class="sxs-lookup"><span data-stu-id="d57f0-112">String</span></span>|<span data-ttu-id="d57f0-113">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="d57f0-113">The display name of the subject.</span></span>|
|<span data-ttu-id="d57f0-114">email</span><span class="sxs-lookup"><span data-stu-id="d57f0-114">email</span></span>|<span data-ttu-id="d57f0-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57f0-115">String</span></span>|<span data-ttu-id="d57f0-116">O endereço de email do assunto.</span><span class="sxs-lookup"><span data-stu-id="d57f0-116">The email address of the subject.</span></span>|
|<span data-ttu-id="d57f0-117">id</span><span class="sxs-lookup"><span data-stu-id="d57f0-117">id</span></span>|<span data-ttu-id="d57f0-118">String</span><span class="sxs-lookup"><span data-stu-id="d57f0-118">String</span></span>| <span data-ttu-id="d57f0-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d57f0-119">Read-only.</span></span>|
|<span data-ttu-id="d57f0-120">objectId</span><span class="sxs-lookup"><span data-stu-id="d57f0-120">objectId</span></span>|<span data-ttu-id="d57f0-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57f0-121">String</span></span>|<span data-ttu-id="d57f0-122">O identificador de objeto do assunto.</span><span class="sxs-lookup"><span data-stu-id="d57f0-122">The object identifier of the subject.</span></span> <span data-ttu-id="d57f0-123">`null` se o assunto ainda não for um usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="d57f0-123">`null` if the subject is not yet a user in the tenant.</span></span>|
|<span data-ttu-id="d57f0-124">principalName</span><span class="sxs-lookup"><span data-stu-id="d57f0-124">principalName</span></span>|<span data-ttu-id="d57f0-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d57f0-125">String</span></span>|<span data-ttu-id="d57f0-126">O nome principal, se conhecido, do assunto.</span><span class="sxs-lookup"><span data-stu-id="d57f0-126">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="d57f0-127">tipo</span><span class="sxs-lookup"><span data-stu-id="d57f0-127">type</span></span>|<span data-ttu-id="d57f0-128">String</span><span class="sxs-lookup"><span data-stu-id="d57f0-128">String</span></span>|<span data-ttu-id="d57f0-129">O tipo de recurso do assunto.</span><span class="sxs-lookup"><span data-stu-id="d57f0-129">The resource type of the subject.</span></span>|
|<span data-ttu-id="d57f0-130">connectedOrganizationId</span><span class="sxs-lookup"><span data-stu-id="d57f0-130">connectedOrganizationId</span></span>|<span data-ttu-id="d57f0-131">String</span><span class="sxs-lookup"><span data-stu-id="d57f0-131">String</span></span>|<span data-ttu-id="d57f0-132">O identificador da organização conectada do assunto.</span><span class="sxs-lookup"><span data-stu-id="d57f0-132">The identifier of the connected organization of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d57f0-133">Relações</span><span class="sxs-lookup"><span data-stu-id="d57f0-133">Relationships</span></span>

| <span data-ttu-id="d57f0-134">Relação</span><span class="sxs-lookup"><span data-stu-id="d57f0-134">Relationship</span></span> | <span data-ttu-id="d57f0-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d57f0-135">Type</span></span>        | <span data-ttu-id="d57f0-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d57f0-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d57f0-137">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="d57f0-137">connectedOrganization</span></span>|[<span data-ttu-id="d57f0-138">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="d57f0-138">connectedOrganization</span></span>](connectedorganization.md)| <span data-ttu-id="d57f0-139">A organização conectada do assunto.</span><span class="sxs-lookup"><span data-stu-id="d57f0-139">The connected organization of the subject.</span></span> <span data-ttu-id="d57f0-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d57f0-140">Read-only.</span></span> <span data-ttu-id="d57f0-141">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d57f0-141">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d57f0-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d57f0-142">JSON representation</span></span>

<span data-ttu-id="d57f0-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d57f0-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
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

