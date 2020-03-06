---
title: tipo de recurso directoryRoleTemplate
description: Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório (directoryRole). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 886c8bf205d3ad8440d708527c12fbe7f565259d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531632"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="2a2b4-105">tipo de recurso directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="2a2b4-105">directoryRoleTemplate resource type</span></span>

<span data-ttu-id="2a2b4-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a2b4-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a2b4-p102">Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório ([directoryRole](directoryrole.md)). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST para o ponto de extremidade `/directoryRoles` com a ID do modelo de função de diretório no qual se baseia a função directory especificada no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida da solicitação, você pode começar a ler e atribuir membros à função de diretório. **Observação**: Um modelo de função de diretório é exposto para a função de diretório Usuários. A função de diretório Users está implícita e não é visível para os clientes de diretório. Todos os usuários do locatário são atribuídos a essa função pela infraestrutura. A função já está ativada. Não use este modelo.</span><span class="sxs-lookup"><span data-stu-id="2a2b4-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="2a2b4-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="2a2b4-119">Methods</span></span>

| <span data-ttu-id="2a2b4-120">Método</span><span class="sxs-lookup"><span data-stu-id="2a2b4-120">Method</span></span>       | <span data-ttu-id="2a2b4-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2a2b4-121">Return Type</span></span>  |<span data-ttu-id="2a2b4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a2b4-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a2b4-123">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="2a2b4-123">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="2a2b4-124">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="2a2b4-124">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="2a2b4-125">Leia as propriedades e os relacionamentos do objeto directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="2a2b4-125">Read properties and relationships of directoryRoleTemplate object.</span></span>|
|[<span data-ttu-id="2a2b4-126">Listar directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="2a2b4-126">List directoryRoleTemplate</span></span>](../api/directoryroletemplate-list.md) | <span data-ttu-id="2a2b4-127">Coleção [directoryRoleTemplate](directoryroletemplate.md)</span><span class="sxs-lookup"><span data-stu-id="2a2b4-127">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="2a2b4-128">Recupere uma lista de objetos directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="2a2b4-128">Retrieve a list of directoryRoleTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a2b4-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a2b4-129">Properties</span></span>
| <span data-ttu-id="2a2b4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a2b4-130">Property</span></span>     | <span data-ttu-id="2a2b4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a2b4-131">Type</span></span>   |<span data-ttu-id="2a2b4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a2b4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a2b4-133">description</span><span class="sxs-lookup"><span data-stu-id="2a2b4-133">description</span></span>|<span data-ttu-id="2a2b4-134">String</span><span class="sxs-lookup"><span data-stu-id="2a2b4-134">String</span></span>|<span data-ttu-id="2a2b4-p103">A descrição definida para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2a2b4-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="2a2b4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2a2b4-137">displayName</span></span>|<span data-ttu-id="2a2b4-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a2b4-138">String</span></span>|<span data-ttu-id="2a2b4-p104">O nome de exibição para definir para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2a2b4-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="2a2b4-141">id</span><span class="sxs-lookup"><span data-stu-id="2a2b4-141">id</span></span>|<span data-ttu-id="2a2b4-142">String</span><span class="sxs-lookup"><span data-stu-id="2a2b4-142">String</span></span>|<span data-ttu-id="2a2b4-p105">O identificador exclusivo do modelo. Herdado de [directoryObject](directoryobject.md). Você especifica a **id** do modelo de função do diretório para a propriedade **roleTemplateId** na solicitação POST para ativar um [directoryRole](directoryrole.md) em um locatário. Chave, Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2a2b4-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a2b4-148">Relações</span><span class="sxs-lookup"><span data-stu-id="2a2b4-148">Relationships</span></span>
<span data-ttu-id="2a2b4-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2a2b4-149">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="2a2b4-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a2b4-150">JSON representation</span></span>

<span data-ttu-id="2a2b4-151">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2a2b4-151">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
