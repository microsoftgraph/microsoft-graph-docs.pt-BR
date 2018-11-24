# <a name="unarchive-team"></a><span data-ttu-id="cb563-101">Equipe de unarchive</span><span class="sxs-lookup"><span data-stu-id="cb563-101">Unarchive team</span></span>



<span data-ttu-id="cb563-102">Restaure uma [equipe](../resources/team.md)de arquivados.</span><span class="sxs-lookup"><span data-stu-id="cb563-102">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="cb563-103">Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe.</span><span class="sxs-lookup"><span data-stu-id="cb563-103">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="cb563-104">As equipes são arquivadas usando o [arquivo morto](team_archive.md) API.</span><span class="sxs-lookup"><span data-stu-id="cb563-104">Teams are archived using the [archive](team_archive.md) API.</span></span>

<span data-ttu-id="cb563-105">Unarchiving é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="cb563-105">Unarchiving is an async operation.</span></span> <span data-ttu-id="cb563-106">Uma equipe é não arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="cb563-106">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb563-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="cb563-107">Permissions</span></span>
<span data-ttu-id="cb563-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb563-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb563-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb563-110">Permission type</span></span>      | <span data-ttu-id="cb563-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb563-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb563-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb563-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cb563-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb563-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb563-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb563-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb563-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb563-115">Not supported.</span></span>    |
|<span data-ttu-id="cb563-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb563-116">Application</span></span> | <span data-ttu-id="cb563-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb563-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="cb563-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb563-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="cb563-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb563-119">Request headers</span></span>
| <span data-ttu-id="cb563-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb563-120">Header</span></span>       | <span data-ttu-id="cb563-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cb563-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb563-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb563-122">Authorization</span></span>  | <span data-ttu-id="cb563-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb563-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb563-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb563-125">Request body</span></span>
<span data-ttu-id="cb563-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb563-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb563-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb563-127">Response</span></span>

<span data-ttu-id="cb563-128">Se unarchiving for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb563-128">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="cb563-129">A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular unarchiving da equipe.</span><span class="sxs-lookup"><span data-stu-id="cb563-129">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="cb563-130">Verificar o status da operação unarchiving fazendo uma solicitação GET para este local.</span><span class="sxs-lookup"><span data-stu-id="cb563-130">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="cb563-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb563-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cb563-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb563-132">Request</span></span>
<span data-ttu-id="cb563-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb563-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="cb563-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb563-134">Response</span></span>
<span data-ttu-id="cb563-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="cb563-135">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
