# <a name="clone-a-team"></a><span data-ttu-id="25fa3-101">Como clonar uma equipe</span><span class="sxs-lookup"><span data-stu-id="25fa3-101">Clone a team</span></span>



<span data-ttu-id="25fa3-102">Crie uma cópia de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="25fa3-102">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="25fa3-103">Esta operação também cria uma cópia do [grupo](../resources/group.md)correspondente.</span><span class="sxs-lookup"><span data-stu-id="25fa3-103">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="25fa3-104">Você pode especificar quais partes da equipe a ser clonada:</span><span class="sxs-lookup"><span data-stu-id="25fa3-104">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="25fa3-105">**apps** - apps cópias equipes da Microsoft que estão instalados na equipe de.</span><span class="sxs-lookup"><span data-stu-id="25fa3-105">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="25fa3-106">**canais** – copia a estrutura de canal (mas não as mensagens no canal).</span><span class="sxs-lookup"><span data-stu-id="25fa3-106">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="25fa3-107">**membros** – copia os membros e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="25fa3-107">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="25fa3-108">**configurações** – copia todas as definições dentro da equipe, juntamente com as configurações de chave de grupo.</span><span class="sxs-lookup"><span data-stu-id="25fa3-108">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="25fa3-109">**guias** – copia as guias no canais.</span><span class="sxs-lookup"><span data-stu-id="25fa3-109">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="25fa3-110">Quando as guias são clonados, eles são colocados em um estado não configurado- - são exibidas na barra de ferramentas guia da Microsoft Teams e, na primeira vez que você abri-los, vá através da tela de configuração.</span><span class="sxs-lookup"><span data-stu-id="25fa3-110">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="25fa3-111">(Se a pessoa que está abrindo a guia não tem permissão para configurar os aplicativos, eles verão uma mensagem que explica que a guia ainda não foram configurada.)</span><span class="sxs-lookup"><span data-stu-id="25fa3-111">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="25fa3-112">A clonagem é uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="25fa3-112">Cloning is a long-running operation.</span></span>
<span data-ttu-id="25fa3-113">Depois que o clone POST retorna, você precisará fazer a [operação](../resources/teamsasyncoperation.md) para verificar se ele está "em execução" ou "sucedidas" ou "Falha".</span><span class="sxs-lookup"><span data-stu-id="25fa3-113">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="25fa3-114">Você deve continuar GET até que o status não é "executando".</span><span class="sxs-lookup"><span data-stu-id="25fa3-114">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="25fa3-115">O atraso recomendado entre obtém é 5 segundos.</span><span class="sxs-lookup"><span data-stu-id="25fa3-115">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="25fa3-116">Permissions</span><span class="sxs-lookup"><span data-stu-id="25fa3-116">Permissions</span></span>

<span data-ttu-id="25fa3-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="25fa3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="25fa3-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25fa3-119">Permission type</span></span>      | <span data-ttu-id="25fa3-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25fa3-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25fa3-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25fa3-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="25fa3-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25fa3-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="25fa3-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25fa3-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25fa3-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25fa3-124">Not supported.</span></span>    |
|<span data-ttu-id="25fa3-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25fa3-125">Application</span></span>                            | <span data-ttu-id="25fa3-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25fa3-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25fa3-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25fa3-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="25fa3-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25fa3-128">Request headers</span></span>
| <span data-ttu-id="25fa3-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25fa3-129">Header</span></span>       | <span data-ttu-id="25fa3-130">Valor</span><span class="sxs-lookup"><span data-stu-id="25fa3-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25fa3-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="25fa3-131">Authorization</span></span>  | <span data-ttu-id="25fa3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25fa3-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="25fa3-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25fa3-134">Content-Type</span></span>  | <span data-ttu-id="25fa3-135">application/json</span><span class="sxs-lookup"><span data-stu-id="25fa3-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25fa3-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25fa3-136">Request body</span></span>

| <span data-ttu-id="25fa3-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25fa3-137">Property</span></span>     | <span data-ttu-id="25fa3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="25fa3-138">Type</span></span>   |<span data-ttu-id="25fa3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="25fa3-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25fa3-140">classificação</span><span class="sxs-lookup"><span data-stu-id="25fa3-140">classification</span></span>|<span data-ttu-id="25fa3-141">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="25fa3-141">String (optional)</span></span>|<span data-ttu-id="25fa3-142">Descreve uma classificação para o grupo (por exemplo, o impacto comercial baixa, média ou alta).</span><span class="sxs-lookup"><span data-stu-id="25fa3-142">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="25fa3-143">Se a classificação não for especificada, a classificação será copiada do team/grupo original.</span><span class="sxs-lookup"><span data-stu-id="25fa3-143">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="25fa3-144">description</span><span class="sxs-lookup"><span data-stu-id="25fa3-144">description</span></span>|<span data-ttu-id="25fa3-145">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="25fa3-145">String (optional)</span></span>|<span data-ttu-id="25fa3-146">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="25fa3-146">An optional description for the group.</span></span> <span data-ttu-id="25fa3-147">Se essa propriedade não for especificada, ele será deixado em branco.</span><span class="sxs-lookup"><span data-stu-id="25fa3-147">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="25fa3-148">displayName</span><span class="sxs-lookup"><span data-stu-id="25fa3-148">displayName</span></span>|<span data-ttu-id="25fa3-149">String</span><span class="sxs-lookup"><span data-stu-id="25fa3-149">String</span></span>|<span data-ttu-id="25fa3-p108">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="25fa3-p108">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="25fa3-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="25fa3-153">mailNickname</span></span>|<span data-ttu-id="25fa3-154">String</span><span class="sxs-lookup"><span data-stu-id="25fa3-154">String</span></span>|<span data-ttu-id="25fa3-155">O alias de email para o grupo, exclusivo na organização.</span><span class="sxs-lookup"><span data-stu-id="25fa3-155">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="25fa3-156">Esta propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="25fa3-156">This property must be specified when a group is created.</span></span> <span data-ttu-id="25fa3-157">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="25fa3-157">Supports $filter.</span></span> <span data-ttu-id="25fa3-158">Se essa propriedade não for especificada, ele será calculado de displayName.</span><span class="sxs-lookup"><span data-stu-id="25fa3-158">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="25fa3-159">Problema conhecido: esta propriedade é ignorada no momento.</span><span class="sxs-lookup"><span data-stu-id="25fa3-159">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="25fa3-160">partsToClone</span><span class="sxs-lookup"><span data-stu-id="25fa3-160">partsToClone</span></span>| [<span data-ttu-id="25fa3-161">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="25fa3-161">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="25fa3-162">Uma lista separada por vírgulas das partes a ser clonada.</span><span class="sxs-lookup"><span data-stu-id="25fa3-162">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="25fa3-163">Partes legais são "apps, guias, configurações, canais, membros".</span><span class="sxs-lookup"><span data-stu-id="25fa3-163">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="25fa3-164">visibilidade</span><span class="sxs-lookup"><span data-stu-id="25fa3-164">visibility</span></span>|<span data-ttu-id="25fa3-165">[teamVisibilityType](../resources/teamVisibilityType.md) (opcional)</span><span class="sxs-lookup"><span data-stu-id="25fa3-165">[teamVisibilityType](../resources/teamVisibilityType.md) (optional)</span></span>| <span data-ttu-id="25fa3-166">Especifica a visibilidade do grupo.</span><span class="sxs-lookup"><span data-stu-id="25fa3-166">Specifies the visibility of the group.</span></span> <span data-ttu-id="25fa3-167">Os valores possíveis são: **particular**e **público**.</span><span class="sxs-lookup"><span data-stu-id="25fa3-167">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="25fa3-168">Se a visibilidade não for especificada, será copiada a visibilidade do team/grupo original.</span><span class="sxs-lookup"><span data-stu-id="25fa3-168">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="25fa3-169">Se a equipe que está sendo clonado é uma equipe **educationClass** , o parâmetro visibilidade será ignorado e visibilidade do novo grupo será definida como HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="25fa3-169">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="25fa3-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="25fa3-170">Response</span></span>

<span data-ttu-id="25fa3-171">Se tiver êxito, este método retornará um `202 Accepted` código de resposta com um local: cabeçalho apontando para o recurso de [operação](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="25fa3-171">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="25fa3-172">Quando a operação for concluída, o recurso de operação informará a id da equipe de criação.</span><span class="sxs-lookup"><span data-stu-id="25fa3-172">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="25fa3-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25fa3-173">Example</span></span>
#### <a name="request"></a><span data-ttu-id="25fa3-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25fa3-174">Request</span></span>
<span data-ttu-id="25fa3-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25fa3-175">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a><span data-ttu-id="25fa3-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="25fa3-176">Response</span></span>
<span data-ttu-id="25fa3-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25fa3-177">The following is an example of the response.</span></span> <span data-ttu-id="25fa3-178">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="25fa3-178">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="25fa3-179">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25fa3-179">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
