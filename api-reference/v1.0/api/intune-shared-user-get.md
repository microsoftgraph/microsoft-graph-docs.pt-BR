---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 909152da2608af14dbcdc693632710e3c6f703dd
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732277"
---
# <a name="get-user"></a><span data-ttu-id="8b112-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="8b112-103">Get user</span></span>

<span data-ttu-id="8b112-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b112-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b112-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b112-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b112-106">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="8b112-106">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b112-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8b112-107">Prerequisites</span></span>
<span data-ttu-id="8b112-108">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8b112-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8b112-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b112-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="8b112-110">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="8b112-110">The specific permission depends on the context.</span></span>

|<span data-ttu-id="8b112-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b112-111">Permission type</span></span>|<span data-ttu-id="8b112-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8b112-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b112-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b112-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8b112-114">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="8b112-114">_varies by context_</span></span>|
| <span data-ttu-id="8b112-115">&nbsp;&nbsp;Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="8b112-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="8b112-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b112-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="8b112-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="8b112-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="8b112-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b112-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="8b112-119">&nbsp;&nbsp;Integração</span><span class="sxs-lookup"><span data-stu-id="8b112-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="8b112-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b112-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8b112-121">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="8b112-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="8b112-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b112-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="8b112-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b112-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b112-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b112-124">Not supported.</span></span>|
|<span data-ttu-id="8b112-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b112-125">Application</span></span>|<span data-ttu-id="8b112-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b112-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b112-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b112-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b112-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8b112-128">Optional query parameters</span></span>
<span data-ttu-id="8b112-129">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8b112-129">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8b112-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b112-130">Request headers</span></span>
|<span data-ttu-id="8b112-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b112-131">Header</span></span>|<span data-ttu-id="8b112-132">Valor</span><span class="sxs-lookup"><span data-stu-id="8b112-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b112-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b112-133">Authorization</span></span>|<span data-ttu-id="8b112-134">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b112-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b112-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8b112-135">Accept</span></span>|<span data-ttu-id="8b112-136">application/json</span><span class="sxs-lookup"><span data-stu-id="8b112-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b112-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b112-137">Request body</span></span>
<span data-ttu-id="8b112-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b112-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b112-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b112-139">Response</span></span>
<span data-ttu-id="8b112-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b112-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b112-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b112-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b112-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b112-142">Request</span></span>
<span data-ttu-id="8b112-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b112-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="8b112-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b112-144">Response</span></span>
<span data-ttu-id="8b112-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b112-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```