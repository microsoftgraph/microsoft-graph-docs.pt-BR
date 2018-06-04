# <a name="share-outlook-message-folders-between-users"></a><span data-ttu-id="2739b-101">Compartilhar pastas de mensagens do Outlook entre usuários</span><span class="sxs-lookup"><span data-stu-id="2739b-101">Share Outlook message folders between users</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="2739b-102">O Outlook permite que clientes compartilhem pastas entre si e forneçam acesso para ler, criar ou modificar pastas individuais ou a caixa de correio inteira.</span><span class="sxs-lookup"><span data-stu-id="2739b-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="2739b-103">Isso também é conhecido como "delegação" no Outlook.</span><span class="sxs-lookup"><span data-stu-id="2739b-103">This is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="2739b-104">O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si.</span><span class="sxs-lookup"><span data-stu-id="2739b-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span>

<span data-ttu-id="2739b-105">Por exemplo, Henrique compartilhou com Diogo sua caixa de entrada com acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="2739b-105">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="2739b-106">Se Diogo estiver conectado em seu aplicativo e tiver fornecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o aplicativo poderá acessar o email e a caixa de entrada do Henrique conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="2739b-106">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="2739b-107">Obter uma mensagem na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="2739b-107">Get a message in the shared folder</span></span>

<span data-ttu-id="2739b-108">Você pode obter uma mensagem específica na caixa de entrada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="2739b-108">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="2739b-109">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [message](../api-reference/v1.0/resources/message.md) identificada por `{id}` da caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="2739b-109">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="2739b-110">Obter todas as mensagens na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="2739b-110">Get all messages in the shared folder</span></span>

<span data-ttu-id="2739b-111">Obtenha todas as mensagens na caixa de entrada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="2739b-111">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="2739b-112">Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [message](../api-reference/v1.0/resources/message.md) na caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="2739b-112">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="2739b-113">Obter a pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="2739b-113">Get the shared folder</span></span>

<span data-ttu-id="2739b-114">Obtenha a pasta (caixa de entrada) que Henrique compartilhou com Diogo.</span><span class="sxs-lookup"><span data-stu-id="2739b-114">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="2739b-115">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [mailFolder](../api-reference/v1.0/resources/mailfolder.md) que representa a pasta de caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="2739b-115">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="2739b-116">Os mesmos recursos de GET se aplicam se Henrique delegar a Diogo mais acesso à sua caixa de entrada ou se Henrique delegar toda a sua caixa de correio a Diogo.</span><span class="sxs-lookup"><span data-stu-id="2739b-116">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="2739b-117">Se Henrique não tiver compartilhado a pasta de mensagens dele com Diogo nem delegado a caixa de correio dele a Diogo, a especificação da ID de usuário do Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="2739b-117">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="2739b-118">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2739b-118">Next steps</span></span>

<span data-ttu-id="2739b-119">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="2739b-119">Find out more about:</span></span>

- [<span data-ttu-id="2739b-120">Por que integrar-se com o email do Outlook</span><span class="sxs-lookup"><span data-stu-id="2739b-120">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="2739b-121">[Como usar a API de email](../api-reference/v1.0/resources/mail_api_overview.md) e seus [casos de uso](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) do Microsoft Graph versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="2739b-121">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>