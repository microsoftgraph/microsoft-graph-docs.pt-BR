---
title: Tipo de recurso accessPackageResourceEnvironment
description: Um ambiente de recurso do pacote de acesso é uma referência ao ambiente de geolocalização no qual um recurso está localizado.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2f03e2c754ea09cdc797b71d4ef59372ac47ff9b
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272515"
---
# <a name="accesspackageresourceenvironment-resource-type"></a><span data-ttu-id="283ae-103">Tipo de recurso accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="283ae-103">accessPackageResourceEnvironment resource type</span></span>

<span data-ttu-id="283ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="283ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="283ae-105">No Gerenciamento de Direitos do [Azure AD,](entitlementmanagement-root.md)um ambiente de recursos do pacote de acesso é uma referência ao ambiente de geolocalização no qual um recurso está localizado.</span><span class="sxs-lookup"><span data-stu-id="283ae-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource environment is a reference to the geolocation environment in which a resource is located.</span></span> <span data-ttu-id="283ae-106">Esse ambiente é fornecido automaticamente como parte do Gerenciamento de Direitos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="283ae-106">This environment is automatically provided as part of Azure AD Entitlement Management.</span></span> <span data-ttu-id="283ae-107">A API só é aplicável a sites multi-geo do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="283ae-107">The API is only applicable to Multi-Geo SharePoint Online sites.</span></span>

## <a name="methods"></a><span data-ttu-id="283ae-108">Methods</span><span class="sxs-lookup"><span data-stu-id="283ae-108">Methods</span></span>
|<span data-ttu-id="283ae-109">Método</span><span class="sxs-lookup"><span data-stu-id="283ae-109">Method</span></span>|<span data-ttu-id="283ae-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="283ae-110">Return type</span></span>|<span data-ttu-id="283ae-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="283ae-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="283ae-112">Listar accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="283ae-112">List accessPackageResourceEnvironments</span></span>](../api/accesspackageresourceenvironment-list.md)|<span data-ttu-id="283ae-113">[Coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="283ae-113">[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection</span></span>|<span data-ttu-id="283ae-114">Recupere uma lista de [objetos accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="283ae-114">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects.</span></span>|
|[<span data-ttu-id="283ae-115">Acessar AccessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="283ae-115">Get accessPackageResourceEnvironment</span></span>](../api/accesspackageresourceenvironment-get.md)|[<span data-ttu-id="283ae-116">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="283ae-116">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="283ae-117">Leia as propriedades e os relacionamentos de um [objeto accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="283ae-117">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="283ae-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="283ae-118">Properties</span></span>
|<span data-ttu-id="283ae-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="283ae-119">Property</span></span>|<span data-ttu-id="283ae-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="283ae-120">Type</span></span>|<span data-ttu-id="283ae-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="283ae-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="283ae-122">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="283ae-122">connectionInfo</span></span>|[<span data-ttu-id="283ae-123">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="283ae-123">connectionInfo</span></span>](../resources/connectioninfo.md)|<span data-ttu-id="283ae-124">Informações de conexão de um ambiente usado para se conectar a um recurso.</span><span class="sxs-lookup"><span data-stu-id="283ae-124">Connection information of an environment used to connect to a resource.</span></span> |
|<span data-ttu-id="283ae-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="283ae-125">createdBy</span></span>|<span data-ttu-id="283ae-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="283ae-126">String</span></span>|<span data-ttu-id="283ae-127">O nome de exibição do usuário que criou esse objeto.</span><span class="sxs-lookup"><span data-stu-id="283ae-127">The display name of the user that created this object.</span></span>|
|<span data-ttu-id="283ae-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="283ae-128">createdDateTime</span></span>|<span data-ttu-id="283ae-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="283ae-129">DateTimeOffset</span></span>|<span data-ttu-id="283ae-130">A data e a hora em que esse objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="283ae-130">The date and time that this object was created.</span></span> <br><span data-ttu-id="283ae-131">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="283ae-131">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="283ae-132">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 `'2014-01-01T00:00:00Z'` será.</span><span class="sxs-lookup"><span data-stu-id="283ae-132">For example, midnight UTC on Jan 1, 2014 is `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="283ae-133">description</span><span class="sxs-lookup"><span data-stu-id="283ae-133">description</span></span>|<span data-ttu-id="283ae-134">String</span><span class="sxs-lookup"><span data-stu-id="283ae-134">String</span></span>|<span data-ttu-id="283ae-135">A descrição deste *objeto accessPackageResourceEnvironment.*</span><span class="sxs-lookup"><span data-stu-id="283ae-135">The description of this *accessPackageResourceEnvironment* object.</span></span>|
|<span data-ttu-id="283ae-136">displayName</span><span class="sxs-lookup"><span data-stu-id="283ae-136">displayName</span></span>|<span data-ttu-id="283ae-137">String</span><span class="sxs-lookup"><span data-stu-id="283ae-137">String</span></span>|<span data-ttu-id="283ae-138">O nome de exibição deste objeto.</span><span class="sxs-lookup"><span data-stu-id="283ae-138">The display name of this object.</span></span>|
|<span data-ttu-id="283ae-139">id</span><span class="sxs-lookup"><span data-stu-id="283ae-139">id</span></span>|<span data-ttu-id="283ae-140">String</span><span class="sxs-lookup"><span data-stu-id="283ae-140">String</span></span>|<span data-ttu-id="283ae-141">O identificador exclusivo atribuído pelo sistema do objeto.</span><span class="sxs-lookup"><span data-stu-id="283ae-141">The system-assigned unique identifier of the object.</span></span>|
|<span data-ttu-id="283ae-142">isDefaultEnvironment</span><span class="sxs-lookup"><span data-stu-id="283ae-142">isDefaultEnvironment</span></span>|<span data-ttu-id="283ae-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="283ae-143">Boolean</span></span>|<span data-ttu-id="283ae-144">Determina se esse é o ambiente padrão ou não.</span><span class="sxs-lookup"><span data-stu-id="283ae-144">Determines whether this is default environment or not.</span></span> <span data-ttu-id="283ae-145">Ele é definido para todos os sistemas de origem estáticos, como grupos do `true` Azure AD e aplicativos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="283ae-145">It is set to `true` for all static origin systems, such as Azure AD groups and Azure AD Applications.</span></span>|
|<span data-ttu-id="283ae-146">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="283ae-146">modifiedBy</span></span>|<span data-ttu-id="283ae-147">String</span><span class="sxs-lookup"><span data-stu-id="283ae-147">String</span></span>|<span data-ttu-id="283ae-148">O nome de exibição da entidade que modificou esse objeto pela última vez.</span><span class="sxs-lookup"><span data-stu-id="283ae-148">The display name of the entity that last modified this object.</span></span>|
|<span data-ttu-id="283ae-149">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="283ae-149">modifiedDateTime</span></span>|<span data-ttu-id="283ae-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="283ae-150">DateTimeOffset</span></span>|<span data-ttu-id="283ae-151">A data e a hora em que esse objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="283ae-151">The date and time that this object was last modified.</span></span> <br><span data-ttu-id="283ae-152">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="283ae-152">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="283ae-153">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 `'2014-01-01T00:00:00Z'` será.</span><span class="sxs-lookup"><span data-stu-id="283ae-153">For example, midnight UTC on Jan 1, 2014 is `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="283ae-154">originId</span><span class="sxs-lookup"><span data-stu-id="283ae-154">originId</span></span>|<span data-ttu-id="283ae-155">String</span><span class="sxs-lookup"><span data-stu-id="283ae-155">String</span></span>|<span data-ttu-id="283ae-156">O identificador exclusivo deste ambiente no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="283ae-156">The unique identifier of this environment in the origin system.</span></span>|
|<span data-ttu-id="283ae-157">originSystem</span><span class="sxs-lookup"><span data-stu-id="283ae-157">originSystem</span></span>|<span data-ttu-id="283ae-158">String</span><span class="sxs-lookup"><span data-stu-id="283ae-158">String</span></span>|<span data-ttu-id="283ae-159">O tipo do recurso no sistema de origem, como `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="283ae-159">The type of the resource in the origin system such as `SharePointOnline`.</span></span> <span data-ttu-id="283ae-160">Oferece suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="283ae-160">Supports `$filter`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="283ae-161">Relações</span><span class="sxs-lookup"><span data-stu-id="283ae-161">Relationships</span></span>
|<span data-ttu-id="283ae-162">Relação</span><span class="sxs-lookup"><span data-stu-id="283ae-162">Relationship</span></span>|<span data-ttu-id="283ae-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="283ae-163">Type</span></span>|<span data-ttu-id="283ae-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="283ae-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="283ae-165">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="283ae-165">accessPackageResources</span></span>|<span data-ttu-id="283ae-166">[Coleção accessPackageResource](../resources/accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="283ae-166">[accessPackageResource](../resources/accesspackageresource.md) collection</span></span>|<span data-ttu-id="283ae-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="283ae-167">Read-only.</span></span> <span data-ttu-id="283ae-168">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="283ae-168">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="283ae-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="283ae-169">JSON representation</span></span>
<span data-ttu-id="283ae-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="283ae-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "originSystem": "String",
  "originId": "String",
  "isDefaultEnvironment": "Boolean",
  "connectionInfo": {
    "@odata.type": "microsoft.graph.connectionInfo"
  },
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```
