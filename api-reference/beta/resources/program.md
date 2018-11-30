---
title: tipo de recurso do programa
description: 'No Windows Azure AD access analisa o recurso, um programa é um contêiner, mantendo os controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para torná-la mais fáceis de localizar relacionados access analisa.  '
ms.openlocfilehash: cb08d0edb7487be95e159ed5e2a2546a92e7bce7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040329"
---
# <a name="program-resource-type"></a><span data-ttu-id="b0c6b-105">tipo de recurso do programa</span><span class="sxs-lookup"><span data-stu-id="b0c6b-105">program resource type</span></span>

> <span data-ttu-id="b0c6b-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0c6b-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0c6b-108">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, um programa é um contêiner, mantendo os controles de programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-108">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="b0c6b-109">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-109">A tenant can have one or more programs.</span></span>  <span data-ttu-id="b0c6b-110">Cada controle vincula uma revisão de acesso a um programa, para torná-la mais fáceis de localizar relacionados access analisa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-110">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="b0c6b-111">Cada locatário que tem em-hospedados Azure AD avaliações de acesso tem um programa, `Default program`.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-111">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="b0c6b-112">Um administrador global pode criar programas adicionais, por exemplo representar as iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-112">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="b0c6b-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0c6b-113">Methods</span></span>

| <span data-ttu-id="b0c6b-114">Método</span><span class="sxs-lookup"><span data-stu-id="b0c6b-114">Method</span></span>           | <span data-ttu-id="b0c6b-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0c6b-115">Return Type</span></span>    |<span data-ttu-id="b0c6b-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c6b-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0c6b-117">Criação de programa</span><span class="sxs-lookup"><span data-stu-id="b0c6b-117">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="b0c6b-118">programa</span><span class="sxs-lookup"><span data-stu-id="b0c6b-118">program</span></span>](program.md)   |   <span data-ttu-id="b0c6b-119">Crie um novo programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-119">Create a new program.</span></span>|
|[<span data-ttu-id="b0c6b-120">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="b0c6b-120">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="b0c6b-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-121">None.</span></span>   |   <span data-ttu-id="b0c6b-122">Exclua um programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-122">Delete a program.</span></span>|
|[<span data-ttu-id="b0c6b-123">Lista de programas</span><span class="sxs-lookup"><span data-stu-id="b0c6b-123">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="b0c6b-124">coleção de [programa](program.md)</span><span class="sxs-lookup"><span data-stu-id="b0c6b-124">[program](program.md) collection</span></span>|   <span data-ttu-id="b0c6b-125">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-125">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="b0c6b-126">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="b0c6b-126">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="b0c6b-127">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="b0c6b-127">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="b0c6b-128">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-128">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="b0c6b-129">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="b0c6b-129">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="b0c6b-130">programa</span><span class="sxs-lookup"><span data-stu-id="b0c6b-130">program</span></span>](program.md)|  <span data-ttu-id="b0c6b-131">Atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-131">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="b0c6b-132">Permissions</span><span class="sxs-lookup"><span data-stu-id="b0c6b-132">Permissions</span></span>

|<span data-ttu-id="b0c6b-133">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0c6b-133">Permission type</span></span>                        | <span data-ttu-id="b0c6b-134">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0c6b-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0c6b-135">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0c6b-135">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0c6b-136">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c6b-136">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="b0c6b-137">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0c6b-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0c6b-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-138">Not supported.</span></span> |
|<span data-ttu-id="b0c6b-139">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0c6b-139">Application</span></span>                            | <span data-ttu-id="b0c6b-140">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-140">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="b0c6b-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0c6b-141">Properties</span></span>
| <span data-ttu-id="b0c6b-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0c6b-142">Property</span></span>     | <span data-ttu-id="b0c6b-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c6b-143">Type</span></span>   |<span data-ttu-id="b0c6b-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c6b-144">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="b0c6b-145">O identificador atribuído pelo recurso do programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-145">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="b0c6b-146">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-146">The name of the program.</span></span>  <span data-ttu-id="b0c6b-147">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-147">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="b0c6b-148">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-148">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="b0c6b-149">Relações</span><span class="sxs-lookup"><span data-stu-id="b0c6b-149">Relationships</span></span>
| <span data-ttu-id="b0c6b-150">Relação</span><span class="sxs-lookup"><span data-stu-id="b0c6b-150">Relationship</span></span> | <span data-ttu-id="b0c6b-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c6b-151">Type</span></span>   |<span data-ttu-id="b0c6b-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c6b-152">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="b0c6b-153">programControl</span><span class="sxs-lookup"><span data-stu-id="b0c6b-153">programControl</span></span>](programcontrol.md) | <span data-ttu-id="b0c6b-154">Controles associados com o programa.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-154">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0c6b-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0c6b-155">JSON representation</span></span>

<span data-ttu-id="b0c6b-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0c6b-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->