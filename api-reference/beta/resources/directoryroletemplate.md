---
title: tipo de recurso directoryRoleTemplate
description: 'Representa um modelo de função de diretório. Um modelo de função directory Especifica os valores de propriedade de uma função de diretório (directoryRole). Há um objeto de modelo de função de diretório associado para cada uma das funções do diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino. Por padrão, apenas a função do diretório de administradores de empresa é ativada. Para ativar a outras funções de diretório disponível você enviar uma solicitação POST para o `/directoryRoles` ponto de extremidade com a ID do modelo de função de diretório no qual a função de diretório se baseia especificado no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida dessa solicitação, você pode iniciar, em seguida, ler e atribuir membros da função de diretório. **Observação**: um modelo de função de diretório é exposto para a função do diretório de usuários. A função do diretório de usuários é implícita e não é visível para os clientes de diretório. Cada usuário no locatário é atribuído a essa função pela infra-estrutura. A função já está ativada. Não use esse modelo.'
ms.openlocfilehash: 088b630a05044f4b3dba59dd1ff6c9a11dce6c0f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033160"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="7d7a9-114">tipo de recurso directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="7d7a9-114">directoryRoleTemplate resource type</span></span>

> <span data-ttu-id="7d7a9-115">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d7a9-115">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d7a9-116">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d7a9-116">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d7a9-p103">Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório ([directoryRole](directoryrole.md)). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST para o ponto de extremidade `/directoryRoles` com a ID do modelo de função de diretório no qual se baseia a função directory especificada no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida da solicitação, você pode começar a ler e atribuir membros à função de diretório. **Observação**: Um modelo de função de diretório é exposto para a função de diretório Usuários. A função de diretório Users está implícita e não é visível para os clientes de diretório. Todos os usuários do locatário são atribuídos a essa função pela infraestrutura. A função já está ativada. Não use este modelo.</span><span class="sxs-lookup"><span data-stu-id="7d7a9-p103">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="7d7a9-129">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d7a9-129">Methods</span></span>

| <span data-ttu-id="7d7a9-130">Método</span><span class="sxs-lookup"><span data-stu-id="7d7a9-130">Method</span></span>       | <span data-ttu-id="7d7a9-131">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d7a9-131">Return Type</span></span>  |<span data-ttu-id="7d7a9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d7a9-132">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d7a9-133">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="7d7a9-133">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="7d7a9-134">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="7d7a9-134">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="7d7a9-135">Leia as propriedades e os relacionamentos do objeto directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="7d7a9-135">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d7a9-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d7a9-136">Properties</span></span>
| <span data-ttu-id="7d7a9-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d7a9-137">Property</span></span>     | <span data-ttu-id="7d7a9-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d7a9-138">Type</span></span>   |<span data-ttu-id="7d7a9-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d7a9-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d7a9-140">description</span><span class="sxs-lookup"><span data-stu-id="7d7a9-140">description</span></span>|<span data-ttu-id="7d7a9-141">String</span><span class="sxs-lookup"><span data-stu-id="7d7a9-141">String</span></span>|<span data-ttu-id="7d7a9-p104">A descrição definida para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d7a9-p104">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="7d7a9-144">displayName</span><span class="sxs-lookup"><span data-stu-id="7d7a9-144">displayName</span></span>|<span data-ttu-id="7d7a9-145">String</span><span class="sxs-lookup"><span data-stu-id="7d7a9-145">String</span></span>|<span data-ttu-id="7d7a9-p105">O nome de exibição para definir para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d7a9-p105">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="7d7a9-148">id</span><span class="sxs-lookup"><span data-stu-id="7d7a9-148">id</span></span>|<span data-ttu-id="7d7a9-149">String</span><span class="sxs-lookup"><span data-stu-id="7d7a9-149">String</span></span>|<span data-ttu-id="7d7a9-p106">O identificador exclusivo do modelo. Herdado de [directoryObject](directoryobject.md). Você especifica a **id** do modelo de função do diretório para a propriedade **roleTemplateId** na solicitação POST para ativar um [directoryRole](directoryrole.md) em um locatário. Chave, Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d7a9-p106">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d7a9-155">Relações</span><span class="sxs-lookup"><span data-stu-id="7d7a9-155">Relationships</span></span>
<span data-ttu-id="7d7a9-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d7a9-156">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="7d7a9-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d7a9-157">JSON representation</span></span>

<span data-ttu-id="7d7a9-158">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7d7a9-158">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
