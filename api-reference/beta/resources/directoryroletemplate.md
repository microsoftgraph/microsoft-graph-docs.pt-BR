---
title: tipo de recurso directoryRoleTemplate
description: 'Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório (directoryRole). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST para o ponto de extremidade `/directoryRoles` com a ID do modelo de função de diretório no qual se baseia a função directory especificada no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida da solicitação, você pode começar a ler e atribuir membros à função de diretório. **Observação**: Um modelo de função de diretório é exposto para a função de diretório Usuários. A função de diretório Users está implícita e não é visível para os clientes de diretório. Todos os usuários do locatário são atribuídos a essa função pela infraestrutura. A função já está ativada. Não use este modelo.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd813c9f7676e7190e5aedbb6d9b950e9ffc6aac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543263"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="74b2f-114">tipo de recurso directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="74b2f-114">directoryRoleTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74b2f-p102">Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório ([directoryRole](directoryrole.md)). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST para o ponto de extremidade `/directoryRoles` com a ID do modelo de função de diretório no qual se baseia a função directory especificada no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida da solicitação, você pode começar a ler e atribuir membros à função de diretório. **Observação**: Um modelo de função de diretório é exposto para a função de diretório Usuários. A função de diretório Users está implícita e não é visível para os clientes de diretório. Todos os usuários do locatário são atribuídos a essa função pela infraestrutura. A função já está ativada. Não use este modelo.</span><span class="sxs-lookup"><span data-stu-id="74b2f-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="74b2f-127">Métodos</span><span class="sxs-lookup"><span data-stu-id="74b2f-127">Methods</span></span>

| <span data-ttu-id="74b2f-128">Método</span><span class="sxs-lookup"><span data-stu-id="74b2f-128">Method</span></span>       | <span data-ttu-id="74b2f-129">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74b2f-129">Return Type</span></span>  |<span data-ttu-id="74b2f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="74b2f-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74b2f-131">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="74b2f-131">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="74b2f-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="74b2f-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="74b2f-133">Leia as propriedades e os relacionamentos do objeto directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="74b2f-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74b2f-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74b2f-134">Properties</span></span>
| <span data-ttu-id="74b2f-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74b2f-135">Property</span></span>     | <span data-ttu-id="74b2f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="74b2f-136">Type</span></span>   |<span data-ttu-id="74b2f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="74b2f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74b2f-138">description</span><span class="sxs-lookup"><span data-stu-id="74b2f-138">description</span></span>|<span data-ttu-id="74b2f-139">String</span><span class="sxs-lookup"><span data-stu-id="74b2f-139">String</span></span>|<span data-ttu-id="74b2f-p103">A descrição definida para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74b2f-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="74b2f-142">displayName</span><span class="sxs-lookup"><span data-stu-id="74b2f-142">displayName</span></span>|<span data-ttu-id="74b2f-143">String</span><span class="sxs-lookup"><span data-stu-id="74b2f-143">String</span></span>|<span data-ttu-id="74b2f-p104">O nome de exibição para definir para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74b2f-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="74b2f-146">id</span><span class="sxs-lookup"><span data-stu-id="74b2f-146">id</span></span>|<span data-ttu-id="74b2f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74b2f-147">String</span></span>|<span data-ttu-id="74b2f-p105">O identificador exclusivo do modelo. Herdado de [directoryObject](directoryobject.md). Você especifica a **id** do modelo de função do diretório para a propriedade **roleTemplateId** na solicitação POST para ativar um [directoryRole](directoryrole.md) em um locatário. Chave, Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74b2f-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74b2f-153">Relações</span><span class="sxs-lookup"><span data-stu-id="74b2f-153">Relationships</span></span>
<span data-ttu-id="74b2f-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74b2f-154">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="74b2f-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74b2f-155">JSON representation</span></span>

<span data-ttu-id="74b2f-156">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="74b2f-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryroletemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
