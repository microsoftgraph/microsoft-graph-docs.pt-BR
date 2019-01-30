---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que podem ser solicitados por um aplicativo cliente chamar outro aplicativo ou que podem ser usadas para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificado. A propriedade **appRoles** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **appRole**.
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640410"
---
# <a name="approle-resource-type"></a><span data-ttu-id="7b529-104">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="7b529-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b529-105">Representa uma função de aplicativo que podem ser solicitados por um aplicativo cliente chamar outro aplicativo ou que podem ser usadas para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="7b529-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="7b529-106">A propriedade **appRoles** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="7b529-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="7b529-107">Importante: Essa funcionalidade está desabilitada na versão atual.</span><span class="sxs-lookup"><span data-stu-id="7b529-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b529-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b529-108">JSON representation</span></span>

<span data-ttu-id="7b529-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7b529-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="7b529-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b529-110">Properties</span></span>
| <span data-ttu-id="7b529-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b529-111">Property</span></span>     | <span data-ttu-id="7b529-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b529-112">Type</span></span>   |<span data-ttu-id="7b529-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b529-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b529-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="7b529-114">allowedMemberTypes</span></span>|<span data-ttu-id="7b529-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b529-115">String collection</span></span>|<span data-ttu-id="7b529-116">Especifica se esta definição de aplicativo de função pode ser atribuída aos usuários e grupos pela configuração para "User", ou para outros aplicativos (que estão acessando este aplicativo em cenários de serviço daemon) por configuração para "Aplicativo", ou ambos.</span><span class="sxs-lookup"><span data-stu-id="7b529-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="7b529-117">description</span><span class="sxs-lookup"><span data-stu-id="7b529-117">description</span></span>|<span data-ttu-id="7b529-118">String</span><span class="sxs-lookup"><span data-stu-id="7b529-118">String</span></span>|<span data-ttu-id="7b529-119">Permissão ajudam o texto que aparece na atribuição app admin e experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="7b529-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="7b529-120">displayName</span><span class="sxs-lookup"><span data-stu-id="7b529-120">displayName</span></span>|<span data-ttu-id="7b529-121">String</span><span class="sxs-lookup"><span data-stu-id="7b529-121">String</span></span>|<span data-ttu-id="7b529-122">Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="7b529-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="7b529-123">id</span><span class="sxs-lookup"><span data-stu-id="7b529-123">id</span></span>|<span data-ttu-id="7b529-124">Guid</span><span class="sxs-lookup"><span data-stu-id="7b529-124">Guid</span></span>|<span data-ttu-id="7b529-125">Identificador exclusivo de função dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="7b529-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="7b529-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7b529-126">isEnabled</span></span>|<span data-ttu-id="7b529-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b529-127">Boolean</span></span>|<span data-ttu-id="7b529-128">Ao criar ou atualizar uma definição de função, isso deve ser definido como **true** (o que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="7b529-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="7b529-129">Para excluir uma função, isso deve primeiro ser definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="7b529-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="7b529-130">Nesse momento, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="7b529-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="7b529-131">valor</span><span class="sxs-lookup"><span data-stu-id="7b529-131">value</span></span>|<span data-ttu-id="7b529-132">String</span><span class="sxs-lookup"><span data-stu-id="7b529-132">String</span></span>|<span data-ttu-id="7b529-133">Especifica o valor da declaração funções que o aplicativo deve esperar em tokens de acesso e autenticação.</span><span class="sxs-lookup"><span data-stu-id="7b529-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
