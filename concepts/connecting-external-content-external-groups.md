---
title: Usar grupos externos para gerenciar permissões para o Microsoft Graph de dados do conector
description: Saiba mais sobre grupos externos para gerenciar permissões para itens externos.
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 8a0ae00e7fc4d1509c29bfb204aae0ab3166970e
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781178"
---
# <a name="use-external-groups-to-manage-permissions-to-microsoft-graph-connector-data-sources"></a><span data-ttu-id="f1802-103">Usar grupos externos para gerenciar permissões para o Microsoft Graph de dados do conector</span><span class="sxs-lookup"><span data-stu-id="f1802-103">Use external groups to manage permissions to Microsoft Graph connector data sources</span></span>

<span data-ttu-id="f1802-104">[Grupos externos](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) permitem gerenciar [](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) permissões para exibir itens externos em uma conexão do Microsoft Graph e se conectar a fontes de dados fora dos grupos Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f1802-104">[External groups](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) allow you to manage permissions to view [external items](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) in a Microsoft Graph connection, and connect to data sources outside Azure Active Directory (Azure AD) groups.</span></span>

<span data-ttu-id="f1802-105">Para fontes de dados que dependem de usuários e grupos do Azure AD, você configura permissões em itens externos associando uma [](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true) lista de controle de acesso (ACL) a um usuário do Azure AD e uma ID de grupo, ao criar ou atualizar os itens externos.</span><span class="sxs-lookup"><span data-stu-id="f1802-105">For data sources that rely on Azure AD users and groups, you set permissions on external items by associating an access control list (ACL) with an Azure AD user and group ID, when [creating](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true) or updating the external items.</span></span>

<span data-ttu-id="f1802-106">No entanto, para fontes de dados que usam grupos que não são do Azure AD ou construções como grupos, como Perfis de Salesforce, Unidades de Negócios Dinâmicas, grupos SharePoint, grupos locais serviceNow ou grupos locais confluência, recomendamos que você use grupos *externos*.</span><span class="sxs-lookup"><span data-stu-id="f1802-106">However, for data sources that use non-Azure AD groups, or group-like constructs, like Salesforce Profiles, Dynamics Business Units, SharePoint groups, ServiceNow local groups, or Confluence local groups, we recommend that you use *external groups*.</span></span>

## <a name="common-external-group-scenarios"></a><span data-ttu-id="f1802-107">Cenários comuns de grupo externo</span><span class="sxs-lookup"><span data-stu-id="f1802-107">Common external group scenarios</span></span>

<span data-ttu-id="f1802-108">A seguir estão exemplos comuns de grupo não específicos do aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1802-108">The following are common non-Azure AD application-specific group examples.</span></span>

<span data-ttu-id="f1802-109">O Microsoft Dynamics 365 permite que os clientes estruturam suas CRMs com unidades de negócios e equipes.</span><span class="sxs-lookup"><span data-stu-id="f1802-109">Microsoft Dynamics 365 allows customers to structure their CRMs with business units and teams.</span></span><span data-ttu-id="f1802-110">As informações de associação para essas unidades de negócios e equipes não são armazenadas no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1802-110"> The membership information for these business units and teams is not stored in Azure AD.</span></span>

<span data-ttu-id="f1802-111">A imagem a seguir mostra a estrutura das unidades de negócios e equipes.</span><span class="sxs-lookup"><span data-stu-id="f1802-111">The following image shows the structure of the business units and teams.</span></span>

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/bu-teams-D365.png" alt="Diagram of an structure in Dynamics 365. A business unit has a team and a manager under it. This manager has other users." style="width:400px;"/></p>

<span data-ttu-id="f1802-112">Salesforce usa perfis, funções e conjuntos de permissões para autorização.</span><span class="sxs-lookup"><span data-stu-id="f1802-112">Salesforce uses profiles, roles, and permission sets for authorization.</span></span> <span data-ttu-id="f1802-113">Elas são específicas do Salesforce e as informações de associação não estão disponíveis no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1802-113">These are specific to Salesforce, and the membership information is not available in Azure AD.</span></span>

<span data-ttu-id="f1802-114">A imagem a seguir mostra a estrutura das informações de associação no Salesforce.</span><span class="sxs-lookup"><span data-stu-id="f1802-114">The following image shows the structure of the membership information in Salesforce.</span></span>

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/roles-salesforce.png" alt="Diagram of an structure of roles in Salesforce. The role of vicepresident of sales is at the top level of the hierarchy, it has three subordinates, namely, the head of sales operations, the head of sales, and the head of account managament. The head of sales at the same time has a sales operations manager as subordinate. And the head of sales has a sales development manager as subordinate." style="width:400px;"/></p>

## <a name="using-external-groups-in-your-connection"></a><span data-ttu-id="f1802-115">Usando grupos externos em sua conexão</span><span class="sxs-lookup"><span data-stu-id="f1802-115">Using external groups in your connection</span></span>

<span data-ttu-id="f1802-116">Para usar grupos externos em suas conexões:</span><span class="sxs-lookup"><span data-stu-id="f1802-116">To use external groups in your connections:</span></span>

1. <span data-ttu-id="f1802-117">Para cada grupo que não seja do Azure AD, crie um grupo externo no Microsoft Graph usando a [API de grupos.](/en-us/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="f1802-117">For each non-Azure AD group, create an external group in Microsoft Graph using the [groups API](/en-us/graph/api/resources/group?view=graph-rest-beta&preserve-view=true).</span></span>
2. <span data-ttu-id="f1802-118">Use o grupo externo ao definir a ACL para seus itens externos, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="f1802-118">Use the external group when defining the ACL for your external items as necessary.</span></span>  
3. <span data-ttu-id="f1802-119">Mantenha a associação dos grupos externos atualizada e em sincronia.</span><span class="sxs-lookup"><span data-stu-id="f1802-119">Keep the membership of the external groups up to date and in sync.</span></span>

### <a name="create-external-groups"></a><span data-ttu-id="f1802-120">Criar grupos externos</span><span class="sxs-lookup"><span data-stu-id="f1802-120">Create external groups</span></span>

<span data-ttu-id="f1802-121">Grupos externos pertencem a uma conexão.</span><span class="sxs-lookup"><span data-stu-id="f1802-121">External groups belong to a connection.</span></span> <span data-ttu-id="f1802-122">Para criar grupos externos em suas conexões:</span><span class="sxs-lookup"><span data-stu-id="f1802-122">To create external groups in your connections:</span></span>
* <span data-ttu-id="f1802-123">Use a API de grupos no Microsoft Graph, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="f1802-123">Use the groups API in Microsoft Graph, as shown in the following example.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f1802-124">[DisplayName](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) e **descrição** são campos opcionais.</span><span class="sxs-lookup"><span data-stu-id="f1802-124">The [displayName](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) and **description** are optional fields.</span></span>

    ```http
    POST /connections/{connectionId}/groups 

    {  
      "id": "contosoEscalations",  
      "displayName": "Contoso Escalations",  
      "description": "Tier-1 escalations within Contoso"
    }  
    ```

* <span data-ttu-id="f1802-125">Forneça um identificador ou um nome no [campo ID.](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="f1802-125">Provide either an identifier or a name in the [ID](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) field.</span></span> <span data-ttu-id="f1802-126">Use esse valor para chamar o grupo externo em solicitações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="f1802-126">Use this value to call the external group in subsequent requests.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f1802-127">O campo ID permite que você use conjuntos de caracteres base64 de URL e nome de arquivo seguro, e ele tem um limite de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f1802-127">The ID field allows you to use URL and filename-safe Base64 character sets, and it has a limit of 128 characters.</span></span>

<span data-ttu-id="f1802-128">Um grupo externo pode conter um ou mais dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="f1802-128">An external group can contain one or more of the following:</span></span>
* <span data-ttu-id="f1802-129">Um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1802-129">An Azure AD user.</span></span>
* <span data-ttu-id="f1802-130">Um grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1802-130">An Azure AD group.</span></span>
* <span data-ttu-id="f1802-131">Outro grupo externo, incluindo grupos externos aninhados.</span><span class="sxs-lookup"><span data-stu-id="f1802-131">Another external group, including nested external groups.</span></span>

<span data-ttu-id="f1802-132">Depois de criar o grupo, você pode adicionar membros ao grupo, conforme mostrado nos exemplos a seguir.</span><span class="sxs-lookup"><span data-stu-id="f1802-132">After you create the group, you can add members to the group, as shown in the following examples.</span></span>

```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members

{ 
  "id": "contosoSupport", 
  "type": "group", 
  "identitySource": "external" 
}
```
```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members 

{ 
  "id": "25f143de-be82-4afb-8a57-e032b9315752", 
  "type": "user", 
  "identitySource": "azureActiveDirectory" 
}
```
```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members 

{ 
  "id": "99a3b3d6-71ee-4d21-b08b-4b6f22e3ae4b", 
  "type": "group", 
  "identitySource": "azureActiveDirectory" 
}
```

### <a name="use-external-groups-in-acl"></a><span data-ttu-id="f1802-133">Usar grupos externos no ACL</span><span class="sxs-lookup"><span data-stu-id="f1802-133">Use external groups in ACL</span></span>

<span data-ttu-id="f1802-134">Você pode usar grupos externos ao definir ACLs para itens [externos,](connecting-external-content-manage-items.md#access-control-list) conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="f1802-134">You can use external groups when defining [ACLs](connecting-external-content-manage-items.md#access-control-list) for external items, as shown in the following example.</span></span> <span data-ttu-id="f1802-135">Além de usuários e grupos do Azure AD, um item externo pode ter grupos externos em suas entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="f1802-135">In addition to Azure AD users and groups, an external item can have external groups in its access control entries.</span></span>

```http
PUT https://graph.microsoft.com/beta/external/connections/{id}/items/{id}  

Content-type: application/json  
{  
  "@odata.type": "microsoft.graph.externalItem",  
  "acl": [  
    {  
      "type": "group",  
      "value": "contosEscalations",  
      "accessType": "grant",  
      "identitySource": "External"  
    },  
    {  
      "type": "user",  
      "value": "87e9089a-08d5-4d9e-9524-b7bd6be580d5",  
      "accessType": "grant",  
      "identitySource": "azureActiveDirectory"  
    },  
    {  
      "type": "group",  
      "value": "96fbeb4f-f71c-4405-9f0b-1d6988eda2d2",  
      "accessType": "deny",  
      "identitySource": "azureActiveDirectory"  
    }  
  ],  
  "properties": {  
    "title": "Error in the payment gateway",  
    "priority": 1,  
    "assignee": "john@contoso.com"  
  },  
  "content": {  
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",  
    "type": "html"  
  }  
}  
```

> [!NOTE]
> <span data-ttu-id="f1802-136">Você pode usar grupos externos em ACLs mesmo antes que os grupos sejam criados.</span><span class="sxs-lookup"><span data-stu-id="f1802-136">You can use external groups in ACLs even before the groups are created.</span></span>

### <a name="keep-external-group-memberships-in-sync"></a><span data-ttu-id="f1802-137">Manter associações de grupo externos em sincronia</span><span class="sxs-lookup"><span data-stu-id="f1802-137">Keep external group memberships in sync</span></span>

<span data-ttu-id="f1802-138">Mantenha a associação do seu grupo externo atualizada no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f1802-138">Keep the membership of your external group up to date in Microsoft Graph.</span></span> <span data-ttu-id="f1802-139">Quando as associações mudarem em seu grupo personalizado, certifique-se de que a alteração seja refletida no grupo externo em um momento que funcione para suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="f1802-139">When memberships change in your custom group, make sure that the change is reflected in the external group at a time that works for your needs.</span></span>

### <a name="manage-external-groups-and-membership"></a><span data-ttu-id="f1802-140">Gerenciar grupos externos e associação</span><span class="sxs-lookup"><span data-stu-id="f1802-140">Manage external groups and membership</span></span>

<span data-ttu-id="f1802-141">Você pode usar a API de grupos para gerenciar seus grupos externos e associações de grupo.</span><span class="sxs-lookup"><span data-stu-id="f1802-141">You can use the groups API to manage your external groups and group membership.</span></span> <span data-ttu-id="f1802-142">Para obter detalhes, [consulte externalGroup](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) e [externalGroupMember](/graph/api/resources/externalgroupmember?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="f1802-142">For details, see [externalGroup](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) and [externalGroupMember](/graph/api/resources/externalgroupmember?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="see-also"></a><span data-ttu-id="f1802-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="f1802-143">See also</span></span>
<span data-ttu-id="f1802-144">Para saber mais sobre a API de conectores Graph Microsoft, consulte [Working with the connectors API](connecting-external-content-connectors-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="f1802-144">To learn more about the Microsoft Graph connectors API, see [Working with the connectors API](connecting-external-content-connectors-api-overview.md).</span></span>
