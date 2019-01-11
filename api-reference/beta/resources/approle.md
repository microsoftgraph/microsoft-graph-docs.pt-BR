---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que podem ser solicitados por um aplicativo cliente chamar outro aplicativo ou que podem ser usadas para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificado. A propriedade **appRoles** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **appRole**.
localization_priority: Normal
ms.openlocfilehash: 26fe11fc4f0c362de002c205c7e3b95a6ec4a314
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891543"
---
# <a name="approle-resource-type"></a><span data-ttu-id="0734d-104">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="0734d-104">appRole resource type</span></span>

> <span data-ttu-id="0734d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0734d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0734d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0734d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0734d-107">Representa uma função de aplicativo que podem ser solicitados por um aplicativo cliente chamar outro aplicativo ou que podem ser usadas para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="0734d-107">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="0734d-108">A propriedade **appRoles** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="0734d-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="0734d-109">Importante: Essa funcionalidade está desabilitada na versão atual.</span><span class="sxs-lookup"><span data-stu-id="0734d-109">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0734d-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0734d-110">JSON representation</span></span>

<span data-ttu-id="0734d-111">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0734d-111">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0734d-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0734d-112">Properties</span></span>
| <span data-ttu-id="0734d-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0734d-113">Property</span></span>     | <span data-ttu-id="0734d-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="0734d-114">Type</span></span>   |<span data-ttu-id="0734d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="0734d-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0734d-116">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="0734d-116">allowedMemberTypes</span></span>|<span data-ttu-id="0734d-117">String collection</span><span class="sxs-lookup"><span data-stu-id="0734d-117">String collection</span></span>|<span data-ttu-id="0734d-118">Especifica se esta definição de aplicativo de função pode ser atribuída aos usuários e grupos pela configuração para "User", ou para outros aplicativos (que estão acessando este aplicativo em cenários de serviço daemon) por configuração para "Aplicativo", ou ambos.</span><span class="sxs-lookup"><span data-stu-id="0734d-118">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="0734d-119">description</span><span class="sxs-lookup"><span data-stu-id="0734d-119">description</span></span>|<span data-ttu-id="0734d-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0734d-120">String</span></span>|<span data-ttu-id="0734d-121">Permissão ajudam o texto que aparece na atribuição app admin e experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="0734d-121">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="0734d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="0734d-122">displayName</span></span>|<span data-ttu-id="0734d-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0734d-123">String</span></span>|<span data-ttu-id="0734d-124">Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="0734d-124">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="0734d-125">id</span><span class="sxs-lookup"><span data-stu-id="0734d-125">id</span></span>|<span data-ttu-id="0734d-126">Guid</span><span class="sxs-lookup"><span data-stu-id="0734d-126">Guid</span></span>|<span data-ttu-id="0734d-127">Identificador exclusivo de função dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="0734d-127">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="0734d-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0734d-128">isEnabled</span></span>|<span data-ttu-id="0734d-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="0734d-129">Boolean</span></span>|<span data-ttu-id="0734d-130">Ao criar ou atualizar uma definição de função, isso deve ser definido como **true** (o que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="0734d-130">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="0734d-131">Para excluir uma função, isso deve primeiro ser definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="0734d-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="0734d-132">Nesse momento, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="0734d-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="0734d-133">valor</span><span class="sxs-lookup"><span data-stu-id="0734d-133">value</span></span>|<span data-ttu-id="0734d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0734d-134">String</span></span>|<span data-ttu-id="0734d-135">Especifica o valor da declaração funções que o aplicativo deve esperar em tokens de acesso e autenticação.</span><span class="sxs-lookup"><span data-stu-id="0734d-135">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
