# <a name="archive-team"></a><span data-ttu-id="b18c5-101">Equipe de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="b18c5-101">Archive team</span></span>



<span data-ttu-id="b18c5-102">Arquive a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="b18c5-102">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="b18c5-103">Quando uma equipe é arquivada, os usuários podem não mais enviar como mensagens em nenhum canal na equipe de, edite o nome da equipe, descrição ou outras configurações ou em geral, verifique a maioria das alterações para a equipe.</span><span class="sxs-lookup"><span data-stu-id="b18c5-103">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="b18c5-104">As alterações de associação para a equipe continuam a ser permitido.</span><span class="sxs-lookup"><span data-stu-id="b18c5-104">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="b18c5-105">O arquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="b18c5-105">Archiving is an async operation.</span></span> <span data-ttu-id="b18c5-106">Uma equipe será arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="b18c5-106">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="b18c5-107">Para arquivar equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.</span><span class="sxs-lookup"><span data-stu-id="b18c5-107">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="b18c5-108">Para restaurar uma equipe de seu estado arquivado, use a API para [unarchive](team_unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="b18c5-108">To restore a team from its archived state, use the API to [unarchive](team_unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b18c5-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="b18c5-109">Permissions</span></span>
<span data-ttu-id="b18c5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b18c5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b18c5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b18c5-112">Permission type</span></span>      | <span data-ttu-id="b18c5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b18c5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b18c5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b18c5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b18c5-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b18c5-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b18c5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b18c5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b18c5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b18c5-117">Not supported.</span></span>    |
|<span data-ttu-id="b18c5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b18c5-118">Application</span></span> | <span data-ttu-id="b18c5-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b18c5-119">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="b18c5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b18c5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="b18c5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b18c5-121">Request headers</span></span>
| <span data-ttu-id="b18c5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b18c5-122">Header</span></span>       | <span data-ttu-id="b18c5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b18c5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b18c5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b18c5-124">Authorization</span></span>  | <span data-ttu-id="b18c5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b18c5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b18c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b18c5-127">Request body</span></span>
<span data-ttu-id="b18c5-128">Na solicitação, você pode _, opcionalmente,_ inclua o `shouldSetSpoSiteReadOnlyForMembers` parâmetro em um JSON body, da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="b18c5-128">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="b18c5-129">Este parâmetro opcional define se deve definir permissões para os membros da equipe como somente leitura no site do Sharepoint Online associado à equipe.</span><span class="sxs-lookup"><span data-stu-id="b18c5-129">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="b18c5-130">Definir como false ou omitindo o corpo todo resultará nesta etapa sendo ignorada.</span><span class="sxs-lookup"><span data-stu-id="b18c5-130">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="b18c5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b18c5-131">Response</span></span>

<span data-ttu-id="b18c5-132">Se arquivamento for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b18c5-132">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="b18c5-133">A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular o arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="b18c5-133">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="b18c5-134">Verificar o status da operação de arquivamento, tornando uma solicitação GET para este local.</span><span class="sxs-lookup"><span data-stu-id="b18c5-134">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="b18c5-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b18c5-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b18c5-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b18c5-136">Request</span></span>
<span data-ttu-id="b18c5-137">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b18c5-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="b18c5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b18c5-138">Response</span></span>
<span data-ttu-id="b18c5-139">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b18c5-139">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
