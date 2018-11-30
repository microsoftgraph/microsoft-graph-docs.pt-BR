---
title: tipo de recurso de directorySetting
description: Configurações do diretório podem ser criadas com base no directorySettingTemplates disponíveis e alteradas de seus padrões predefinidos. Essas configurações podem controlar comportamentos de entidade ou recurso, em um nível de locatário todo ou em um nível de entidade específica. Quando a mesma configuração é definida no nível de entidade de todo o inquilino e específicos, a configuração de nível de entidade específica pode recusar da configuração de todo o inquilino.  Por exemplo, a configuração de todo o inquilino pode permitir convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir convidados sejam convidados por membros do grupo. Atualmente configurações definidas pelo sistema são apenas regem o comportamento de grupos do Office.
ms.openlocfilehash: 4a807d22bfd5d6651b4064542d33fe285b637a3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036781"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="f621d-107">tipo de recurso de directorySetting</span><span class="sxs-lookup"><span data-stu-id="f621d-107">directorySetting resource type</span></span>

> <span data-ttu-id="f621d-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f621d-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f621d-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f621d-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f621d-110">Configurações do diretório podem ser criadas com base no disponíveis [directorySettingTemplates](directorysettingtemplate.md)e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="f621d-110">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="f621d-111">Essas configurações podem controlar comportamentos de entidade ou recurso, em um nível de locatário todo ou em um nível de entidade específica.</span><span class="sxs-lookup"><span data-stu-id="f621d-111">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="f621d-112">Quando a mesma configuração é definida no nível de entidade de todo o inquilino e específicos, a configuração de nível de entidade específica pode recusar da configuração de todo o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f621d-112">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="f621d-113">Por exemplo, a configuração de todo o inquilino pode permitir convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir convidados sejam convidados por membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="f621d-113">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="f621d-114">Atualmente configurações definidas pelo sistema são apenas regem o comportamento de grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="f621d-114">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="f621d-115">**Observação**: A versão /beta do tipo de recurso directorySetting se aplica apenas aos grupos.</span><span class="sxs-lookup"><span data-stu-id="f621d-115">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="f621d-116">A versão /v1.0 foi renomeada para groupSetting.</span><span class="sxs-lookup"><span data-stu-id="f621d-116">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="f621d-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="f621d-117">Methods</span></span>

| <span data-ttu-id="f621d-118">Método</span><span class="sxs-lookup"><span data-stu-id="f621d-118">Method</span></span>           | <span data-ttu-id="f621d-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f621d-119">Return Type</span></span>    |<span data-ttu-id="f621d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f621d-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f621d-121">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="f621d-121">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="f621d-122">directorySetting</span><span class="sxs-lookup"><span data-stu-id="f621d-122">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="f621d-123">Crie um objeto de configuração com base em um directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="f621d-123">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="f621d-124">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="f621d-124">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="f621d-125">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="f621d-125">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="f621d-126">directorySetting</span><span class="sxs-lookup"><span data-stu-id="f621d-126">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="f621d-127">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="f621d-127">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="f621d-128">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="f621d-128">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="f621d-129">coleção [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="f621d-129">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="f621d-130">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="f621d-130">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="f621d-131">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="f621d-131">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="f621d-132">directorySetting</span><span class="sxs-lookup"><span data-stu-id="f621d-132">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="f621d-133">Atualizar um objeto setting.</span><span class="sxs-lookup"><span data-stu-id="f621d-133">Update a setting object.</span></span> <span data-ttu-id="f621d-134">SettingValues só pode ser alterada em uma atualização.</span><span class="sxs-lookup"><span data-stu-id="f621d-134">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="f621d-135">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="f621d-135">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="f621d-136">None</span><span class="sxs-lookup"><span data-stu-id="f621d-136">None</span></span> |<span data-ttu-id="f621d-137">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="f621d-137">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f621d-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f621d-138">Properties</span></span>
| <span data-ttu-id="f621d-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f621d-139">Property</span></span>     | <span data-ttu-id="f621d-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="f621d-140">Type</span></span>   |<span data-ttu-id="f621d-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="f621d-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f621d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="f621d-142">displayName</span></span>|<span data-ttu-id="f621d-143">string</span><span class="sxs-lookup"><span data-stu-id="f621d-143">string</span></span>|<span data-ttu-id="f621d-144">Nome de exibição deste grupo de configurações, originado do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="f621d-144">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="f621d-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f621d-145">Read-only.</span></span>|
|<span data-ttu-id="f621d-146">id</span><span class="sxs-lookup"><span data-stu-id="f621d-146">id</span></span>|<span data-ttu-id="f621d-147">string</span><span class="sxs-lookup"><span data-stu-id="f621d-147">string</span></span>| <span data-ttu-id="f621d-p108">Identificador exclusivo destas configurações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f621d-p108">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="f621d-150">templateId</span><span class="sxs-lookup"><span data-stu-id="f621d-150">templateId</span></span>|<span data-ttu-id="f621d-151">string</span><span class="sxs-lookup"><span data-stu-id="f621d-151">string</span></span>| <span data-ttu-id="f621d-p109">Identificador exclusivo para o modelo usado para criar este grupo de configurações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f621d-p109">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="f621d-154">values</span><span class="sxs-lookup"><span data-stu-id="f621d-154">values</span></span>|<span data-ttu-id="f621d-155">conjunto [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f621d-155">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="f621d-p110">Conjunto de pares de nome/valor. Deve conter e ajustar todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="f621d-p110">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f621d-158">Relações</span><span class="sxs-lookup"><span data-stu-id="f621d-158">Relationships</span></span>
<span data-ttu-id="f621d-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f621d-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f621d-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f621d-160">JSON representation</span></span>

<span data-ttu-id="f621d-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f621d-161">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->