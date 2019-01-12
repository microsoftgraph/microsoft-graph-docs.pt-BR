---
title: tipo de recurso directoryRoleTemplate
description: 'Representa um modelo de função de diretório. Um modelo de função directory Especifica os valores de propriedade de uma função de diretório (directoryRole). Há um objeto de modelo de função de diretório associado para cada uma das funções do diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino. Por padrão, apenas a função do diretório de administradores de empresa é ativada. Para ativar a outras funções de diretório disponível você enviar uma solicitação POST para o `/directoryRoles` ponto de extremidade com a ID do modelo de função de diretório no qual a função de diretório se baseia especificado no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida dessa solicitação, você pode iniciar, em seguida, ler e atribuir membros da função de diretório. **Observação**: um modelo de função de diretório é exposto para a função do diretório de usuários. A função do diretório de usuários é implícita e não é visível para os clientes de diretório. Cada usuário no locatário é atribuído a essa função pela infra-estrutura. A função já está ativada. Não use esse modelo.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b4a4e79c11f38991da88cd685983229c9f7da7b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938178"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="ddd6e-114">tipo de recurso directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="ddd6e-114">directoryRoleTemplate resource type</span></span>

> <span data-ttu-id="ddd6e-115">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ddd6e-115">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddd6e-116">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ddd6e-116">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddd6e-p103">Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório ([directoryRole](directoryrole.md)). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST para o ponto de extremidade `/directoryRoles` com a ID do modelo de função de diretório no qual se baseia a função directory especificada no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida da solicitação, você pode começar a ler e atribuir membros à função de diretório. **Observação**: Um modelo de função de diretório é exposto para a função de diretório Usuários. A função de diretório Users está implícita e não é visível para os clientes de diretório. Todos os usuários do locatário são atribuídos a essa função pela infraestrutura. A função já está ativada. Não use este modelo.</span><span class="sxs-lookup"><span data-stu-id="ddd6e-p103">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="ddd6e-129">Métodos</span><span class="sxs-lookup"><span data-stu-id="ddd6e-129">Methods</span></span>

| <span data-ttu-id="ddd6e-130">Método</span><span class="sxs-lookup"><span data-stu-id="ddd6e-130">Method</span></span>       | <span data-ttu-id="ddd6e-131">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ddd6e-131">Return Type</span></span>  |<span data-ttu-id="ddd6e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddd6e-132">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ddd6e-133">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="ddd6e-133">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="ddd6e-134">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="ddd6e-134">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="ddd6e-135">Leia as propriedades e os relacionamentos do objeto directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="ddd6e-135">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddd6e-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddd6e-136">Properties</span></span>
| <span data-ttu-id="ddd6e-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddd6e-137">Property</span></span>     | <span data-ttu-id="ddd6e-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddd6e-138">Type</span></span>   |<span data-ttu-id="ddd6e-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddd6e-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddd6e-140">description</span><span class="sxs-lookup"><span data-stu-id="ddd6e-140">description</span></span>|<span data-ttu-id="ddd6e-141">String</span><span class="sxs-lookup"><span data-stu-id="ddd6e-141">String</span></span>|<span data-ttu-id="ddd6e-p104">A descrição definida para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ddd6e-p104">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="ddd6e-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ddd6e-144">displayName</span></span>|<span data-ttu-id="ddd6e-145">String</span><span class="sxs-lookup"><span data-stu-id="ddd6e-145">String</span></span>|<span data-ttu-id="ddd6e-p105">O nome de exibição para definir para a função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ddd6e-p105">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="ddd6e-148">id</span><span class="sxs-lookup"><span data-stu-id="ddd6e-148">id</span></span>|<span data-ttu-id="ddd6e-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddd6e-149">String</span></span>|<span data-ttu-id="ddd6e-p106">O identificador exclusivo do modelo. Herdado de [directoryObject](directoryobject.md). Você especifica a **id** do modelo de função do diretório para a propriedade **roleTemplateId** na solicitação POST para ativar um [directoryRole](directoryrole.md) em um locatário. Chave, Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ddd6e-p106">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddd6e-155">Relações</span><span class="sxs-lookup"><span data-stu-id="ddd6e-155">Relationships</span></span>
<span data-ttu-id="ddd6e-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ddd6e-156">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="ddd6e-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddd6e-157">JSON representation</span></span>

<span data-ttu-id="ddd6e-158">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ddd6e-158">Here is a JSON representation of the resource</span></span>

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
