---
title: tipo de recurso de directorySetting
description: Configurações do diretório podem ser criadas com base no directorySettingTemplates disponíveis e alteradas de seus padrões predefinidos. Essas configurações podem controlar comportamentos de entidade ou recurso, em um nível de locatário todo ou em um nível de entidade específica. Quando a mesma configuração é definida no nível de entidade de todo o inquilino e específicos, a configuração de nível de entidade específica pode recusar da configuração de todo o inquilino.  Por exemplo, a configuração de todo o inquilino pode permitir convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir convidados sejam convidados por membros do grupo. Atualmente configurações definidas pelo sistema são apenas regem o comportamento de grupos do Office.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521366"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="53a42-107">tipo de recurso de directorySetting</span><span class="sxs-lookup"><span data-stu-id="53a42-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53a42-108">Configurações do diretório podem ser criadas com base no disponíveis [directorySettingTemplates](directorysettingtemplate.md)e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="53a42-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="53a42-109">Essas configurações podem controlar comportamentos de entidade ou recurso, em um nível de locatário todo ou em um nível de entidade específica.</span><span class="sxs-lookup"><span data-stu-id="53a42-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="53a42-110">Quando a mesma configuração é definida no nível de entidade de todo o inquilino e específicos, a configuração de nível de entidade específica pode recusar da configuração de todo o inquilino.</span><span class="sxs-lookup"><span data-stu-id="53a42-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="53a42-111">Por exemplo, a configuração de todo o inquilino pode permitir convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir convidados sejam convidados por membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="53a42-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="53a42-112">Atualmente configurações definidas pelo sistema são apenas regem o comportamento de grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="53a42-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="53a42-113">**Observação**: A versão /beta do tipo de recurso directorySetting se aplica apenas aos grupos.</span><span class="sxs-lookup"><span data-stu-id="53a42-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="53a42-114">A versão /v1.0 foi renomeada para groupSetting.</span><span class="sxs-lookup"><span data-stu-id="53a42-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="53a42-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="53a42-115">Methods</span></span>

| <span data-ttu-id="53a42-116">Método</span><span class="sxs-lookup"><span data-stu-id="53a42-116">Method</span></span>           | <span data-ttu-id="53a42-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="53a42-117">Return Type</span></span>    |<span data-ttu-id="53a42-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="53a42-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53a42-119">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="53a42-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="53a42-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="53a42-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="53a42-121">Crie um objeto de configuração com base em um directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="53a42-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="53a42-122">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="53a42-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="53a42-123">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="53a42-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="53a42-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="53a42-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="53a42-125">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="53a42-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="53a42-126">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="53a42-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="53a42-127">conjunto [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="53a42-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="53a42-128">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="53a42-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="53a42-129">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="53a42-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="53a42-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="53a42-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="53a42-131">Atualizar um objeto setting.</span><span class="sxs-lookup"><span data-stu-id="53a42-131">Update a setting object.</span></span> <span data-ttu-id="53a42-132">SettingValues só pode ser alterada em uma atualização.</span><span class="sxs-lookup"><span data-stu-id="53a42-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="53a42-133">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="53a42-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="53a42-134">None</span><span class="sxs-lookup"><span data-stu-id="53a42-134">None</span></span> |<span data-ttu-id="53a42-135">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="53a42-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="53a42-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53a42-136">Properties</span></span>
| <span data-ttu-id="53a42-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53a42-137">Property</span></span>     | <span data-ttu-id="53a42-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="53a42-138">Type</span></span>   |<span data-ttu-id="53a42-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="53a42-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53a42-140">displayName</span><span class="sxs-lookup"><span data-stu-id="53a42-140">displayName</span></span>|<span data-ttu-id="53a42-141">string</span><span class="sxs-lookup"><span data-stu-id="53a42-141">string</span></span>|<span data-ttu-id="53a42-142">Nome de exibição deste grupo de configurações, originado do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="53a42-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="53a42-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53a42-143">Read-only.</span></span>|
|<span data-ttu-id="53a42-144">id</span><span class="sxs-lookup"><span data-stu-id="53a42-144">id</span></span>|<span data-ttu-id="53a42-145">string</span><span class="sxs-lookup"><span data-stu-id="53a42-145">string</span></span>| <span data-ttu-id="53a42-p107">Identificador exclusivo destas configurações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53a42-p107">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="53a42-148">templateId</span><span class="sxs-lookup"><span data-stu-id="53a42-148">templateId</span></span>|<span data-ttu-id="53a42-149">string</span><span class="sxs-lookup"><span data-stu-id="53a42-149">string</span></span>| <span data-ttu-id="53a42-p108">Identificador exclusivo para o modelo usado para criar este grupo de configurações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53a42-p108">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="53a42-152">values</span><span class="sxs-lookup"><span data-stu-id="53a42-152">values</span></span>|<span data-ttu-id="53a42-153">conjunto [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="53a42-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="53a42-p109">Conjunto de pares de nome/valor. Deve conter e ajustar todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="53a42-p109">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53a42-156">Relações</span><span class="sxs-lookup"><span data-stu-id="53a42-156">Relationships</span></span>
<span data-ttu-id="53a42-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53a42-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="53a42-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53a42-158">JSON representation</span></span>

<span data-ttu-id="53a42-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53a42-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
