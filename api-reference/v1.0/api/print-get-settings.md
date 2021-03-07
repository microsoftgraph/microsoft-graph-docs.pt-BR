---
title: Obter printSettings
description: Recupere as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f7899af4ea72307a4f9c725d131601d30cf90317
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516932"
---
# <a name="get-printsettings"></a><span data-ttu-id="5e893-103">Obter printSettings</span><span class="sxs-lookup"><span data-stu-id="5e893-103">Get printSettings</span></span>

<span data-ttu-id="5e893-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e893-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5e893-105">Recupere as configurações de todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="5e893-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e893-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e893-106">Permissions</span></span>
<span data-ttu-id="5e893-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e893-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5e893-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5e893-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="5e893-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="5e893-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="5e893-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e893-111">Permission type</span></span> | <span data-ttu-id="5e893-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e893-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5e893-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e893-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5e893-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e893-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="5e893-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e893-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e893-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e893-116">Not Supported.</span></span>|
|<span data-ttu-id="5e893-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e893-117">Application</span></span>|<span data-ttu-id="5e893-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e893-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e893-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e893-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e893-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5e893-120">Optional query parameters</span></span>
<span data-ttu-id="5e893-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5e893-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5e893-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5e893-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e893-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e893-123">Request headers</span></span>
| <span data-ttu-id="5e893-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5e893-124">Name</span></span>      |<span data-ttu-id="5e893-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e893-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e893-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e893-126">Authorization</span></span> | <span data-ttu-id="5e893-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e893-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e893-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e893-129">Request body</span></span>
<span data-ttu-id="5e893-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e893-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e893-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e893-131">Response</span></span>
<span data-ttu-id="5e893-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printSettings](../resources/printsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e893-132">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e893-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5e893-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e893-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e893-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/settings
```


### <a name="response"></a><span data-ttu-id="5e893-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e893-135">Response</span></span>
<span data-ttu-id="5e893-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e893-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

