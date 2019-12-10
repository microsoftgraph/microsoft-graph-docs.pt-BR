---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9893edff219e4c0e3a2018f653dcb8dbee11885
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939484"
---
# <a name="get-user"></a><span data-ttu-id="6bb0f-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="6bb0f-103">Get user</span></span>

> <span data-ttu-id="6bb0f-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6bb0f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bb0f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bb0f-107">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6bb0f-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bb0f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bb0f-108">Prerequisites</span></span>

<span data-ttu-id="6bb0f-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6bb0f-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bb0f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6bb0f-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="6bb0f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bb0f-112">Permission type</span></span>|<span data-ttu-id="6bb0f-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bb0f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bb0f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bb0f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6bb0f-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6bb0f-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6bb0f-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bb0f-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="6bb0f-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="6bb0f-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="6bb0f-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bb0f-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="6bb0f-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="6bb0f-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6bb0f-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bb0f-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6bb0f-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="6bb0f-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="6bb0f-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bb0f-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="6bb0f-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bb0f-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bb0f-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-124">Not supported.</span></span>|
|<span data-ttu-id="6bb0f-125">Application</span><span class="sxs-lookup"><span data-stu-id="6bb0f-125">Application</span></span>||
| <span data-ttu-id="6bb0f-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6bb0f-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6bb0f-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bb0f-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="6bb0f-128">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="6bb0f-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="6bb0f-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bb0f-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="6bb0f-130">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="6bb0f-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6bb0f-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bb0f-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6bb0f-132">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="6bb0f-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="6bb0f-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bb0f-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bb0f-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb0f-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6bb0f-135">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6bb0f-135">Optional query parameters</span></span>

<span data-ttu-id="6bb0f-136">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-136">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bb0f-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb0f-137">Request headers</span></span>

|<span data-ttu-id="6bb0f-138">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bb0f-138">Header</span></span>|<span data-ttu-id="6bb0f-139">Valor</span><span class="sxs-lookup"><span data-stu-id="6bb0f-139">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bb0f-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bb0f-140">Authorization</span></span>|<span data-ttu-id="6bb0f-141">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-141">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bb0f-142">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bb0f-142">Accept</span></span>|<span data-ttu-id="6bb0f-143">application/json</span><span class="sxs-lookup"><span data-stu-id="6bb0f-143">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bb0f-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb0f-144">Request body</span></span>

<span data-ttu-id="6bb0f-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bb0f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bb0f-146">Response</span></span>

<span data-ttu-id="6bb0f-147">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-147">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bb0f-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bb0f-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bb0f-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb0f-149">Request</span></span>

<span data-ttu-id="6bb0f-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-150">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="6bb0f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bb0f-151">Response</span></span>

<span data-ttu-id="6bb0f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bb0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











