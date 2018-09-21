# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="935ac-101">Obter mensagens do Outlook em uma pasta compartilhada ou delegada</span><span class="sxs-lookup"><span data-stu-id="935ac-101">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="935ac-102">Permite que os clientes do Outlook compartilhem pastas de email entre si e fornece acesso para "ler", "criar", "modificar" ou "excluir" pastas individuais.</span><span class="sxs-lookup"><span data-stu-id="935ac-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="935ac-103">O Outlook também permite que um cliente delegue a outro usuário permissão para agir em seu nome e acessar pastas de email específicas ou toda a caixa de correio do cliente; Isso também é conhecido como "delegação" no Outlook.</span><span class="sxs-lookup"><span data-stu-id="935ac-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="935ac-104">O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si.</span><span class="sxs-lookup"><span data-stu-id="935ac-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="935ac-105">O suporte também se aplica às pastas que foram delegadas.</span><span class="sxs-lookup"><span data-stu-id="935ac-105">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="935ac-106">Por exemplo, Garth compartilhou a sua caixa de entrada com John e lhe deu acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="935ac-106">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="935ac-107">Se John estiver conectado no seu aplicativo e tiver fornecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o seu aplicativo poderá acessar o email e a caixa de entrada de Garth, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="935ac-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="935ac-108">Obter uma mensagem na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="935ac-108">Get a message in the shared folder</span></span>

<span data-ttu-id="935ac-109">Você pode obter uma mensagem específica na caixa de entrada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="935ac-109">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="935ac-110">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [message](../api-reference/v1.0/resources/message.md) identificada por `{id}` da caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="935ac-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="935ac-111">Obter todas as mensagens na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="935ac-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="935ac-112">Obtenha todas as mensagens na caixa de entrada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="935ac-112">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="935ac-113">Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [message](../api-reference/v1.0/resources/message.md) na caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="935ac-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="935ac-114">Obter a pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="935ac-114">Get the shared folder</span></span>

<span data-ttu-id="935ac-115">Obtenha a pasta (caixa de entrada) que Henrique compartilhou com Diogo.</span><span class="sxs-lookup"><span data-stu-id="935ac-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="935ac-116">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [mailFolder](../api-reference/v1.0/resources/mailfolder.md) que representa a pasta de caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="935ac-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="935ac-117">Os mesmos recursos de GET se aplicam se Henrique delegar a Diogo mais acesso à sua caixa de entrada ou se Henrique delegar toda a sua caixa de correio a Diogo.</span><span class="sxs-lookup"><span data-stu-id="935ac-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="935ac-118">Se Garth não tiver compartilhado sua caixa de entrada com John, nem delegado sua caixa de correio para John, especificar a identificação de usuário de Garth ou nome UPN nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="935ac-118">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="935ac-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="935ac-119">Next steps</span></span>

<span data-ttu-id="935ac-120">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="935ac-120">Find out more about:</span></span>

- [<span data-ttu-id="935ac-121">Por que integrar-se com o email do Outlook</span><span class="sxs-lookup"><span data-stu-id="935ac-121">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="935ac-122">[Como usar a API de email](../api-reference/v1.0/resources/mail_api_overview.md) e seus [casos de uso](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) do Microsoft Graph versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="935ac-122">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>