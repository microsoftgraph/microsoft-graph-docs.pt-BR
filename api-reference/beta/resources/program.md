---
title: tipo de recurso do programa
description: 'No Windows Azure AD access analisa o recurso, um programa é um contêiner, mantendo os controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para torná-la mais fáceis de localizar relacionados access analisa.  '
localization_priority: Normal
ms.openlocfilehash: a342fd159bba3f7e31c55ffab9a64a72353bc7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863900"
---
# <a name="program-resource-type"></a><span data-ttu-id="aafef-105">tipo de recurso do programa</span><span class="sxs-lookup"><span data-stu-id="aafef-105">program resource type</span></span>

> <span data-ttu-id="aafef-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aafef-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aafef-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aafef-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aafef-108">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, um programa é um contêiner, mantendo os controles de programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-108">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="aafef-109">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="aafef-109">A tenant can have one or more programs.</span></span>  <span data-ttu-id="aafef-110">Cada controle vincula uma revisão de acesso a um programa, para torná-la mais fáceis de localizar relacionados access analisa.</span><span class="sxs-lookup"><span data-stu-id="aafef-110">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="aafef-111">Cada locatário que tem em-hospedados Azure AD avaliações de acesso tem um programa, `Default program`.</span><span class="sxs-lookup"><span data-stu-id="aafef-111">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="aafef-112">Um administrador global pode criar programas adicionais, por exemplo representar as iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="aafef-112">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="aafef-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="aafef-113">Methods</span></span>

| <span data-ttu-id="aafef-114">Método</span><span class="sxs-lookup"><span data-stu-id="aafef-114">Method</span></span>           | <span data-ttu-id="aafef-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aafef-115">Return Type</span></span>    |<span data-ttu-id="aafef-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="aafef-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aafef-117">Criação de programa</span><span class="sxs-lookup"><span data-stu-id="aafef-117">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="aafef-118">programa</span><span class="sxs-lookup"><span data-stu-id="aafef-118">program</span></span>](program.md)   |   <span data-ttu-id="aafef-119">Crie um novo programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-119">Create a new program.</span></span>|
|[<span data-ttu-id="aafef-120">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="aafef-120">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="aafef-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aafef-121">None.</span></span>   |   <span data-ttu-id="aafef-122">Exclua um programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-122">Delete a program.</span></span>|
|[<span data-ttu-id="aafef-123">Lista de programas</span><span class="sxs-lookup"><span data-stu-id="aafef-123">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="aafef-124">coleção de [programa](program.md)</span><span class="sxs-lookup"><span data-stu-id="aafef-124">[program](program.md) collection</span></span>|   <span data-ttu-id="aafef-125">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="aafef-125">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="aafef-126">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="aafef-126">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="aafef-127">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="aafef-127">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="aafef-128">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-128">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="aafef-129">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="aafef-129">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="aafef-130">programa</span><span class="sxs-lookup"><span data-stu-id="aafef-130">program</span></span>](program.md)|  <span data-ttu-id="aafef-131">Atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-131">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="aafef-132">Permissions</span><span class="sxs-lookup"><span data-stu-id="aafef-132">Permissions</span></span>

|<span data-ttu-id="aafef-133">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aafef-133">Permission type</span></span>                        | <span data-ttu-id="aafef-134">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aafef-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aafef-135">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aafef-135">Delegated (work or school account)</span></span>     | <span data-ttu-id="aafef-136">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aafef-136">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="aafef-137">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aafef-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aafef-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aafef-138">Not supported.</span></span> |
|<span data-ttu-id="aafef-139">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aafef-139">Application</span></span>                            | <span data-ttu-id="aafef-140">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aafef-140">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="aafef-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aafef-141">Properties</span></span>
| <span data-ttu-id="aafef-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aafef-142">Property</span></span>     | <span data-ttu-id="aafef-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="aafef-143">Type</span></span>   |<span data-ttu-id="aafef-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="aafef-144">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="aafef-145">O identificador atribuído pelo recurso do programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-145">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="aafef-146">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-146">The name of the program.</span></span>  <span data-ttu-id="aafef-147">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="aafef-147">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="aafef-148">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-148">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="aafef-149">Relações</span><span class="sxs-lookup"><span data-stu-id="aafef-149">Relationships</span></span>
| <span data-ttu-id="aafef-150">Relação</span><span class="sxs-lookup"><span data-stu-id="aafef-150">Relationship</span></span> | <span data-ttu-id="aafef-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="aafef-151">Type</span></span>   |<span data-ttu-id="aafef-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="aafef-152">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="aafef-153">programControl</span><span class="sxs-lookup"><span data-stu-id="aafef-153">programControl</span></span>](programcontrol.md) | <span data-ttu-id="aafef-154">Controles associados com o programa.</span><span class="sxs-lookup"><span data-stu-id="aafef-154">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aafef-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aafef-155">JSON representation</span></span>

<span data-ttu-id="aafef-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aafef-156">Here is a JSON representation of the resource.</span></span>

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
