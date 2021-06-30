---
title: Tipo de recurso cloudPcAuditActor
description: O ator de auditoria representado pelo usuário e aplicativo do Azure AD associado ao evento de auditoria.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c0c63e9e9d0db7a5227f0ab7b818c8ab3d3944d9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211194"
---
# <a name="cloudpcauditactor-resource-type"></a><span data-ttu-id="5cf11-103">Tipo de recurso cloudPcAuditActor</span><span class="sxs-lookup"><span data-stu-id="5cf11-103">cloudPcAuditActor resource type</span></span>

<span data-ttu-id="5cf11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cf11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf11-105">O ator de auditoria representado pelo usuário e aplicativo do Azure AD associado ao evento de auditoria.</span><span class="sxs-lookup"><span data-stu-id="5cf11-105">The audit actor represented by the Azure AD user and application associated with the audit event.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="5cf11-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cf11-106">Properties</span></span>

|<span data-ttu-id="5cf11-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cf11-107">Property</span></span>|<span data-ttu-id="5cf11-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cf11-108">Type</span></span>|<span data-ttu-id="5cf11-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cf11-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cf11-110">type</span><span class="sxs-lookup"><span data-stu-id="5cf11-110">type</span></span>|[<span data-ttu-id="5cf11-111">cloudPcAuditActorType</span><span class="sxs-lookup"><span data-stu-id="5cf11-111">cloudPcAuditActorType</span></span>](#cloudpcauditactortype-values)|<span data-ttu-id="5cf11-112">O tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="5cf11-112">The actor type.</span></span> <span data-ttu-id="5cf11-113">Os valores possíveis `ItPro` `Application` incluem , e `Partner` `Unknown` .</span><span class="sxs-lookup"><span data-stu-id="5cf11-113">Possible values include `ItPro`, `Application`, `Partner` and `Unknown`.</span></span>|
|<span data-ttu-id="5cf11-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="5cf11-114">userPermissions</span></span>|<span data-ttu-id="5cf11-115">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf11-115">String collection</span></span>|<span data-ttu-id="5cf11-116">Lista de permissões de usuário e permissões de aplicativo quando o evento de auditoria foi executado.</span><span class="sxs-lookup"><span data-stu-id="5cf11-116">List of user permissions and application permissions when the audit event was performed.</span></span>|
|<span data-ttu-id="5cf11-117">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="5cf11-117">applicationId</span></span>|<span data-ttu-id="5cf11-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf11-118">String</span></span>|<span data-ttu-id="5cf11-119">ID do aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5cf11-119">Azure AD application ID.</span></span>|
|<span data-ttu-id="5cf11-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="5cf11-120">applicationDisplayName</span></span>|<span data-ttu-id="5cf11-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf11-121">String</span></span>|<span data-ttu-id="5cf11-122">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5cf11-122">Name of the application.</span></span>|
|<span data-ttu-id="5cf11-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5cf11-123">userPrincipalName</span></span>|<span data-ttu-id="5cf11-124">String</span><span class="sxs-lookup"><span data-stu-id="5cf11-124">String</span></span>|<span data-ttu-id="5cf11-125">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="5cf11-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="5cf11-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="5cf11-126">servicePrincipalName</span></span>|<span data-ttu-id="5cf11-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf11-127">String</span></span>|<span data-ttu-id="5cf11-128">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="5cf11-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="5cf11-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5cf11-129">ipAddress</span></span>|<span data-ttu-id="5cf11-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf11-130">String</span></span>|<span data-ttu-id="5cf11-131">Endereço IP.</span><span class="sxs-lookup"><span data-stu-id="5cf11-131">IP address.</span></span>|
|<span data-ttu-id="5cf11-132">userId</span><span class="sxs-lookup"><span data-stu-id="5cf11-132">userId</span></span>|<span data-ttu-id="5cf11-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf11-133">String</span></span>|<span data-ttu-id="5cf11-134">ID do usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5cf11-134">Azure AD user ID.</span></span>|
|<span data-ttu-id="5cf11-135">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="5cf11-135">userRoleScopeTags</span></span>|<span data-ttu-id="5cf11-136">[Coleção cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="5cf11-136">[cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md) collection</span></span>|<span data-ttu-id="5cf11-137">Lista de marcas de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="5cf11-137">List of role scope tags.</span></span>|
|<span data-ttu-id="5cf11-138">remoteTenantId</span><span class="sxs-lookup"><span data-stu-id="5cf11-138">remoteTenantId</span></span>|<span data-ttu-id="5cf11-139">String</span><span class="sxs-lookup"><span data-stu-id="5cf11-139">String</span></span>|<span data-ttu-id="5cf11-140">A ID do locatário do parceiro delegado.</span><span class="sxs-lookup"><span data-stu-id="5cf11-140">The delegated partner tenant ID.</span></span>|
|<span data-ttu-id="5cf11-141">remoteUserId</span><span class="sxs-lookup"><span data-stu-id="5cf11-141">remoteUserId</span></span>|<span data-ttu-id="5cf11-142">String</span><span class="sxs-lookup"><span data-stu-id="5cf11-142">String</span></span>|<span data-ttu-id="5cf11-143">A ID de usuário do parceiro delegada.</span><span class="sxs-lookup"><span data-stu-id="5cf11-143">The delegated partner user ID.</span></span>|

### <a name="cloudpcauditactortype-values"></a><span data-ttu-id="5cf11-144">valores cloudPcAuditActorType</span><span class="sxs-lookup"><span data-stu-id="5cf11-144">cloudPcAuditActorType values</span></span>

|<span data-ttu-id="5cf11-145">Member</span><span class="sxs-lookup"><span data-stu-id="5cf11-145">Member</span></span>|<span data-ttu-id="5cf11-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cf11-146">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5cf11-147">itPro</span><span class="sxs-lookup"><span data-stu-id="5cf11-147">itPro</span></span>|<span data-ttu-id="5cf11-148">A operação foi realizada por um profissional de IT.</span><span class="sxs-lookup"><span data-stu-id="5cf11-148">The operation was performed by an IT pro.</span></span>|
|<span data-ttu-id="5cf11-149">aplicação</span><span class="sxs-lookup"><span data-stu-id="5cf11-149">application</span></span>|<span data-ttu-id="5cf11-150">A operação foi executada pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5cf11-150">The operation was performed by the application.</span></span>|
|<span data-ttu-id="5cf11-151">partner</span><span class="sxs-lookup"><span data-stu-id="5cf11-151">partner</span></span>|<span data-ttu-id="5cf11-152">A operação foi realizada por um parceiro.</span><span class="sxs-lookup"><span data-stu-id="5cf11-152">The operation was performed by a partner.</span></span>|
|<span data-ttu-id="5cf11-153">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5cf11-153">unknown</span></span>|<span data-ttu-id="5cf11-154">Ator desconhecido.</span><span class="sxs-lookup"><span data-stu-id="5cf11-154">Unknown actor.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cf11-155">Relações</span><span class="sxs-lookup"><span data-stu-id="5cf11-155">Relationships</span></span>

<span data-ttu-id="5cf11-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cf11-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cf11-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cf11-157">JSON Representation</span></span>

<span data-ttu-id="5cf11-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cf11-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditActor"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```
