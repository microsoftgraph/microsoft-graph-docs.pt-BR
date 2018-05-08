# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="9cb0e-101">Tipo de recurso mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="9cb0e-101">mailboxSettings resource type</span></span>

<span data-ttu-id="9cb0e-102">Configurações para a caixa de correio principal do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9cb0e-102">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="9cb0e-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cb0e-103">Properties</span></span>
| <span data-ttu-id="9cb0e-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cb0e-104">Property</span></span>     | <span data-ttu-id="9cb0e-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cb0e-105">Type</span></span>   |<span data-ttu-id="9cb0e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cb0e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cb0e-107">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="9cb0e-107">archiveFolder</span></span>|<span data-ttu-id="9cb0e-108">string</span><span class="sxs-lookup"><span data-stu-id="9cb0e-108">string</span></span>|<span data-ttu-id="9cb0e-109">ID de uma pasta de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="9cb0e-109">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="9cb0e-110">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9cb0e-110">automaticRepliesSetting</span></span>|[<span data-ttu-id="9cb0e-111">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9cb0e-111">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="9cb0e-112">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9cb0e-112">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="9cb0e-113">idioma</span><span class="sxs-lookup"><span data-stu-id="9cb0e-113">language</span></span>|[<span data-ttu-id="9cb0e-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="9cb0e-114">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="9cb0e-115">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="9cb0e-115">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="9cb0e-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="9cb0e-116">timeZone</span></span>|<span data-ttu-id="9cb0e-117">string</span><span class="sxs-lookup"><span data-stu-id="9cb0e-117">string</span></span>|<span data-ttu-id="9cb0e-118">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="9cb0e-118">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="9cb0e-119">workingHours</span><span class="sxs-lookup"><span data-stu-id="9cb0e-119">workingHours</span></span>|[<span data-ttu-id="9cb0e-120">workingHours</span><span class="sxs-lookup"><span data-stu-id="9cb0e-120">workingHours</span></span>](workinghours.md)|<span data-ttu-id="9cb0e-121">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="9cb0e-121">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cb0e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cb0e-122">JSON representation</span></span>

<span data-ttu-id="9cb0e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cb0e-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->