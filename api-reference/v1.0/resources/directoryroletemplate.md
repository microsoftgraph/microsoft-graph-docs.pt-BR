---
title: tipo de recurso directoryRoleTemplate
description: 'Representa um modelo de função de diretório. Um modelo de função directory Especifica os valores de propriedade de uma função de diretório (directoryRole). Há um objeto de modelo de função de diretório associado para cada uma das funções do diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino. Por padrão, apenas a função do diretório de administradores de empresa é ativada. Para ativar a outras funções de diretório disponível você enviar uma solicitação POST para o `/directoryRoles` ponto de extremidade com a ID do modelo de função de diretório no qual a função de diretório se baseia especificado no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida dessa solicitação, você pode iniciar, em seguida, ler e atribuir membros da função de diretório. **Observação**: um modelo de função de diretório é exposto para a função do diretório de usuários. A função do diretório de usuários é implícita e não é visível para os clientes de diretório. Cada usuário no locatário é atribuído a essa função pela infra-estrutura. A função já está ativada. Não use esse modelo.'
ms.openlocfilehash: e654ab8c14a0c5e831b2cbf818047fea0e2d95c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006504"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="d3fec-114">tipo de recurso directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="d3fec-114">directoryRoleTemplate resource type</span></span>

<span data-ttu-id="d3fec-p102">Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório ([directoryRole](directoryrole.md)). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST para o ponto de extremidade `/directoryRoles` com a ID do modelo de função de diretório no qual se baseia a função directory especificada no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida da solicitação, você pode começar a ler e atribuir membros à função de diretório. **Observação**: Um modelo de função de diretório é exposto para a função de diretório Usuários. A função de diretório Users está implícita e não é visível para os clientes de diretório. Todos os usuários do locatário são atribuídos a essa função pela infraestrutura. A função já está ativada. Não use este modelo.</span><span class="sxs-lookup"><span data-stu-id="d3fec-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="d3fec-127">Métodos</span><span class="sxs-lookup"><span data-stu-id="d3fec-127">Methods</span></span>

| <span data-ttu-id="d3fec-128">Método</span><span class="sxs-lookup"><span data-stu-id="d3fec-128">Method</span></span>       | <span data-ttu-id="d3fec-129">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d3fec-129">Return Type</span></span>  |<span data-ttu-id="d3fec-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3fec-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3fec-131">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="d3fec-131">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="d3fec-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="d3fec-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="d3fec-133">Leia as propriedades e os relacionamentos do objeto directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="d3fec-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|
|[<span data-ttu-id="d3fec-134">List directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="d3fec-134">List directoryRoleTemplate</span></span>](../api/directoryroletemplate-list.md) | <span data-ttu-id="d3fec-135">Coleção [directoryRoleTemplate](directoryroletemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d3fec-135">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="d3fec-136">Recupere uma lista de objetos directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="d3fec-136">Retrieve a list of directoryRoleTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3fec-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3fec-137">Properties</span></span>
| <span data-ttu-id="d3fec-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3fec-138">Property</span></span>     | <span data-ttu-id="d3fec-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3fec-139">Type</span></span>   |<span data-ttu-id="d3fec-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3fec-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3fec-141">description</span><span class="sxs-lookup"><span data-stu-id="d3fec-141">description</span></span>|<span data-ttu-id="d3fec-142">String</span><span class="sxs-lookup"><span data-stu-id="d3fec-142">String</span></span>|<span data-ttu-id="d3fec-p103">A descrição definida para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3fec-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="d3fec-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d3fec-145">displayName</span></span>|<span data-ttu-id="d3fec-146">String</span><span class="sxs-lookup"><span data-stu-id="d3fec-146">String</span></span>|<span data-ttu-id="d3fec-p104">O nome de exibição para definir para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3fec-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="d3fec-149">id</span><span class="sxs-lookup"><span data-stu-id="d3fec-149">id</span></span>|<span data-ttu-id="d3fec-150">String</span><span class="sxs-lookup"><span data-stu-id="d3fec-150">String</span></span>|<span data-ttu-id="d3fec-p105">O identificador exclusivo do modelo. Herdado de [directoryObject](directoryobject.md). Você especifica a **id** do modelo de função do diretório para a propriedade **roleTemplateId** na solicitação POST para ativar um [directoryRole](directoryrole.md) em um locatário. Chave, Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3fec-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3fec-156">Relações</span><span class="sxs-lookup"><span data-stu-id="d3fec-156">Relationships</span></span>
<span data-ttu-id="d3fec-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3fec-157">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="d3fec-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3fec-158">JSON representation</span></span>

<span data-ttu-id="d3fec-159">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d3fec-159">Here is a JSON representation of the resource</span></span>

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
