# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="3c96b-101">Obtenha os contatos do Outlook em uma pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="3c96b-101">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="3c96b-102">O Outlook permite que os clientes compartilhem pastas entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" para pastas de contato individuais.</span><span class="sxs-lookup"><span data-stu-id="3c96b-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="3c96b-103">O Outlook também permite que um cliente delegue outro usuário para agir em seu nome e acessar pastas específicas ou toda a caixa de correio dele; Isso também é conhecido como "delegação" no Outlook.</span><span class="sxs-lookup"><span data-stu-id="3c96b-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="3c96b-104">Via programação, o Microsoft Graph oferece suporte para obter contatos em pastas de contatos compartilhadas por outros usuários, além de obter as próprias pastas compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="3c96b-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="3c96b-105">O suporte também se aplica a pastas em uma caixa de correio delegada.</span><span class="sxs-lookup"><span data-stu-id="3c96b-105">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="3c96b-106">Por exemplo, Garth compartilhou com John uma pasta de contato personalizada com acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="3c96b-106">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="3c96b-107">Se John estiver conectado no seu aplicativo e tiver fornecido permissões delegadas (Contacts.Read.Shared ou Contacts.ReadWrite.Shared), o seu aplicativo poderá acessar a pasta de contatos personalizada do Garth e os contatos nela contidos, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="3c96b-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="3c96b-108">Obter um contato na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="3c96b-108">Get a message in the shared folder</span></span>

<span data-ttu-id="3c96b-109">Você pode obter um contato específico na pasta de contato personalizada que Garth compartilhou com John:</span><span class="sxs-lookup"><span data-stu-id="3c96b-109">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="3c96b-110">Após a conclusão bem-sucedida, você obterá HTTP 200 OK e a instância [contact](../api-reference/v1.0/resources/contact.md) identificada por `{id}` da pasta de contatos compartilhada por Garth.</span><span class="sxs-lookup"><span data-stu-id="3c96b-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/contact.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="3c96b-111">Obter todos os contatos na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="3c96b-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="3c96b-112">Obtenha todos os contatos na pasta de contatos compartilhada por Garth:</span><span class="sxs-lookup"><span data-stu-id="3c96b-112">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="3c96b-113">Após a conclusão bem-sucedida, você obterá HTTP 200 OK e uma coleção de instâncias [contact](../api-reference/v1.0/resources/contact.md) na pasta de contatos compartilhada por Garth.</span><span class="sxs-lookup"><span data-stu-id="3c96b-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/contact.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="3c96b-114">Obter a pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="3c96b-114">Get the shared folder</span></span>

<span data-ttu-id="3c96b-115">Obtenha a pasta de contatos que Garth compartilhou com John.</span><span class="sxs-lookup"><span data-stu-id="3c96b-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="3c96b-116">Após a conclusão bem-sucedida, você obterá HTTP 200 OK e uma instância [contactFolder](../api-reference/v1.0/resources/contactfolder.md) que representa a pasta de contatos compartilhada por Garth.</span><span class="sxs-lookup"><span data-stu-id="3c96b-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/contactfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="3c96b-117">Os mesmos recursos GET aplicam se Garth delegadar a John sua caixa de correio inteira.</span><span class="sxs-lookup"><span data-stu-id="3c96b-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="3c96b-118">Se Garth não tiver compartilhado a pasta de contatos com John, nem delegado sua caixa de correio, especificar a identificação de usuário de Garth ou nome UPN nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="3c96b-118">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="3c96b-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3c96b-119">Next steps</span></span>

<span data-ttu-id="3c96b-120">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="3c96b-120">Find out more about:</span></span>

- [<span data-ttu-id="3c96b-121">Por que se integrar aos contatos pessoais do Outlook</span><span class="sxs-lookup"><span data-stu-id="3c96b-121">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="3c96b-122">A [API de Contatos](../api-reference/v1.0/resources/contact.md) no Microsoft Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="3c96b-122">The [contacts API](../api-reference/v1.0/resources/contact.md) in Microsoft Graph v1.0.</span></span>