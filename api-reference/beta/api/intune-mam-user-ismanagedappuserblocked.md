---
title: função isManagedAppUserBlocked
description: Obtém o estado bloqueado de um usuário de aplicativo gerenciado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41b4a113dd2aa774df59368dde15f1b0f11aa84a
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636494"
---
# <a name="ismanagedappuserblocked-function"></a><span data-ttu-id="8da67-103">função isManagedAppUserBlocked</span><span class="sxs-lookup"><span data-stu-id="8da67-103">isManagedAppUserBlocked function</span></span>

> <span data-ttu-id="8da67-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8da67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8da67-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8da67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8da67-106">Obtém o estado bloqueado de um usuário de aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="8da67-106">Gets the blocked state of a managed app user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8da67-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8da67-107">Prerequisites</span></span>
<span data-ttu-id="8da67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8da67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8da67-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8da67-110">Permission type</span></span>|<span data-ttu-id="8da67-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8da67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8da67-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8da67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8da67-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8da67-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8da67-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8da67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8da67-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8da67-115">Not supported.</span></span>|
|<span data-ttu-id="8da67-116">Application</span><span class="sxs-lookup"><span data-stu-id="8da67-116">Application</span></span>|<span data-ttu-id="8da67-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8da67-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8da67-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8da67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/isManagedAppUserBlocked
```

## <a name="request-headers"></a><span data-ttu-id="8da67-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8da67-119">Request headers</span></span>
|<span data-ttu-id="8da67-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8da67-120">Header</span></span>|<span data-ttu-id="8da67-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8da67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8da67-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8da67-122">Authorization</span></span>|<span data-ttu-id="8da67-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8da67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8da67-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8da67-124">Accept</span></span>|<span data-ttu-id="8da67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8da67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8da67-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8da67-126">Request body</span></span>
<span data-ttu-id="8da67-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8da67-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8da67-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8da67-128">Response</span></span>
<span data-ttu-id="8da67-129">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8da67-129">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8da67-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8da67-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8da67-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8da67-131">Request</span></span>
<span data-ttu-id="8da67-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8da67-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/isManagedAppUserBlocked
```

### <a name="response"></a><span data-ttu-id="8da67-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8da67-133">Response</span></span>
<span data-ttu-id="8da67-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8da67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





