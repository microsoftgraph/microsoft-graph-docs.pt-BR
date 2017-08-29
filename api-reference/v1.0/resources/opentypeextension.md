# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="cc62c-101">Tipo de recurso openTypeExtension (extensões abertas)</span><span class="sxs-lookup"><span data-stu-id="cc62c-101">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="cc62c-p101">As extensões abertas (conhecidas anteriormente como extensões de dados do Office 365) fornecem uma maneira fácil de adicionar propriedades não tipadas diretamente a um recurso no Microsoft Graph. Extensões abertas são representadas pelo recurso **openTypeExtension**. Qualquer extensão aberta adicionada a um recurso é mostrada na propriedade de navegação das **extensions**, que deriva do tipo abstrato [extension](extension.md).  Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados. Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`. Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.</span><span class="sxs-lookup"><span data-stu-id="cc62c-p101">Open extensions (formerly known as Office 365 data extensions) gives you an easy way to directly add untyped properties to a resource in Microsoft Graph. Open extensions are represented by the **openTypeExtension** resource. Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.  Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data. One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`. Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="cc62c-108">Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)</span><span class="sxs-lookup"><span data-stu-id="cc62c-108">Open extension example: [Add custom data to users using open extensions](../../../concepts/extensibility_open_users.md)</span></span>

<span data-ttu-id="cc62c-109">As extensões abertas têm suporte nos recursos a seguir nas versões correspondentes - disponibilidade geral (GA: /v1.0 e /beta) ou visualização (/beta).</span><span class="sxs-lookup"><span data-stu-id="cc62c-109">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="cc62c-110">Recurso</span><span class="sxs-lookup"><span data-stu-id="cc62c-110">Resource</span></span> | <span data-ttu-id="cc62c-111">Versão</span><span class="sxs-lookup"><span data-stu-id="cc62c-111">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="cc62c-112">Unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="cc62c-112">Administrative unit</span></span>](../../beta/resources/administrativeunit.md)  | <span data-ttu-id="cc62c-113">Somente para visualização</span><span class="sxs-lookup"><span data-stu-id="cc62c-113">Preview only</span></span> |
| [<span data-ttu-id="cc62c-114">Evento de calendário</span><span class="sxs-lookup"><span data-stu-id="cc62c-114">Calendar event</span></span>](event.md) | <span data-ttu-id="cc62c-115">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-115">GA</span></span> |
| <span data-ttu-id="cc62c-116">[Evento de calendário](event.md) do grupo</span><span class="sxs-lookup"><span data-stu-id="cc62c-116">[Group calendar event](event.md)</span></span> | <span data-ttu-id="cc62c-117">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-117">GA</span></span> |
| <span data-ttu-id="cc62c-118">[Postagem](post.md) de thread de conversa do grupo</span><span class="sxs-lookup"><span data-stu-id="cc62c-118">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="cc62c-119">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-119">GA</span></span> |
| [<span data-ttu-id="cc62c-120">device</span><span class="sxs-lookup"><span data-stu-id="cc62c-120">device</span></span>](device.md) | <span data-ttu-id="cc62c-121">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-121">GA</span></span> |
| [<span data-ttu-id="cc62c-122">group</span><span class="sxs-lookup"><span data-stu-id="cc62c-122">group</span></span>](group.md) | <span data-ttu-id="cc62c-123">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-123">GA</span></span> |
| [<span data-ttu-id="cc62c-124">message</span><span class="sxs-lookup"><span data-stu-id="cc62c-124">message</span></span>](message.md) | <span data-ttu-id="cc62c-125">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-125">GA</span></span> |
| [<span data-ttu-id="cc62c-126">organization</span><span class="sxs-lookup"><span data-stu-id="cc62c-126">organization</span></span>](organization.md) | <span data-ttu-id="cc62c-127">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-127">GA</span></span> |
| [<span data-ttu-id="cc62c-128">Contato pessoal</span><span class="sxs-lookup"><span data-stu-id="cc62c-128">Personal contact</span></span>](contact.md) | <span data-ttu-id="cc62c-129">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-129">GA</span></span> |
| [<span data-ttu-id="cc62c-130">user</span><span class="sxs-lookup"><span data-stu-id="cc62c-130">user</span></span>](user.md) | <span data-ttu-id="cc62c-131">GA</span><span class="sxs-lookup"><span data-stu-id="cc62c-131">GA</span></span> |

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="cc62c-132">Usar extensões abertas (para recursos do Outlook) ou propriedades estendidas?</span><span class="sxs-lookup"><span data-stu-id="cc62c-132">Use open extensions (for Outlook resources) or extended properties?</span></span>

<span data-ttu-id="cc62c-p102">As extensões abertas são a solução recomendada para a maioria dos cenários que envolvem armazenar e acessar dados personalizados. Se, no entanto, você precisar acessar dados personalizados para as propriedades do Outlook MAPI que já não estão expostos por meio dos [metadados da API do Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), você pode usar [as propriedades estendidas e sua API REST](extended-properties-overview.md). Você pode confirmar quais propriedades os metadados expõem em https://graph.microsoft.com/v1.0/$ metadados.</span><span class="sxs-lookup"><span data-stu-id="cc62c-p102">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data. If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md). You can verify which properties the metadata exposes at https://graph.microsoft.com/v1.0/$metadata.</span></span>


## <a name="json-representation"></a><span data-ttu-id="cc62c-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc62c-136">JSON representation</span></span>

<span data-ttu-id="cc62c-137">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cc62c-137">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="cc62c-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc62c-138">Properties</span></span>
| <span data-ttu-id="cc62c-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc62c-139">Property</span></span>     | <span data-ttu-id="cc62c-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc62c-140">Type</span></span>   |<span data-ttu-id="cc62c-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc62c-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc62c-142">extensionName</span><span class="sxs-lookup"><span data-stu-id="cc62c-142">extensionName</span></span>|<span data-ttu-id="cc62c-143">String</span><span class="sxs-lookup"><span data-stu-id="cc62c-143">String</span></span>|<span data-ttu-id="cc62c-p103">Um identificador de texto exclusivo para uma extensão de tipo aberto. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc62c-p103">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="cc62c-146">id</span><span class="sxs-lookup"><span data-stu-id="cc62c-146">id</span></span>|<span data-ttu-id="cc62c-147">String</span><span class="sxs-lookup"><span data-stu-id="cc62c-147">String</span></span>| <span data-ttu-id="cc62c-p104">Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc62c-p104">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc62c-150">Relações</span><span class="sxs-lookup"><span data-stu-id="cc62c-150">Relationships</span></span>
<span data-ttu-id="cc62c-151">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cc62c-151">None</span></span>


## <a name="methods"></a><span data-ttu-id="cc62c-152">Métodos</span><span class="sxs-lookup"><span data-stu-id="cc62c-152">Methods</span></span>

| <span data-ttu-id="cc62c-153">Método</span><span class="sxs-lookup"><span data-stu-id="cc62c-153">Method</span></span>           | <span data-ttu-id="cc62c-154">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc62c-154">Return Type</span></span>    |<span data-ttu-id="cc62c-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc62c-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc62c-156">Post</span><span class="sxs-lookup"><span data-stu-id="cc62c-156">Post</span></span>](../api/opentypeextension_post_opentypeextension.md) | <span data-ttu-id="cc62c-157">[openTypeExtension](opentypeextension.md) (em uma instância de recurso existente) ou um novo [contato](../resources/contact.md), [evento](../resources/event.md) ou [mensagem](../resources/message.md) que contenha um objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="cc62c-157">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="cc62c-158">Crie um objeto openTypeExtension em uma instância de recurso novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="cc62c-158">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="cc62c-159">Get</span><span class="sxs-lookup"><span data-stu-id="cc62c-159">Get</span></span>](../api/opentypeextension_get.md) | [<span data-ttu-id="cc62c-160">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="cc62c-160">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="cc62c-161">Leia propriedades e relações do objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="cc62c-161">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="cc62c-162">Update</span><span class="sxs-lookup"><span data-stu-id="cc62c-162">Update</span></span>](../api/opentypeextension_update.md) | [<span data-ttu-id="cc62c-163">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="cc62c-163">openTypeExtension</span></span>](opentypeextension.md)   |<span data-ttu-id="cc62c-164">Atualize o objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="cc62c-164">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="cc62c-165">Delete</span><span class="sxs-lookup"><span data-stu-id="cc62c-165">Delete</span></span>](../api/opentypeextension_delete.md) | <span data-ttu-id="cc62c-166">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cc62c-166">None</span></span> |<span data-ttu-id="cc62c-167">Exclua um objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="cc62c-167">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->