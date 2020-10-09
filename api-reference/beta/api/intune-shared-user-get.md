---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae68a269837a8c774102be3655714f47a20715da
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404039"
---
# <a name="get-user"></a><span data-ttu-id="6f8ee-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="6f8ee-103">Get user</span></span>

<span data-ttu-id="6f8ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f8ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f8ee-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f8ee-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f8ee-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f8ee-108">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ee-108">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f8ee-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f8ee-109">Prerequisites</span></span>

<span data-ttu-id="6f8ee-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6f8ee-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f8ee-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6f8ee-112">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="6f8ee-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f8ee-113">Permission type</span></span>|<span data-ttu-id="6f8ee-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f8ee-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f8ee-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f8ee-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f8ee-116">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="6f8ee-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6f8ee-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f8ee-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="6f8ee-118">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="6f8ee-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="6f8ee-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f8ee-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="6f8ee-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="6f8ee-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6f8ee-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f8ee-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6f8ee-122">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="6f8ee-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="6f8ee-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f8ee-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="6f8ee-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f8ee-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f8ee-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-125">Not supported.</span></span>|
|<span data-ttu-id="6f8ee-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f8ee-126">Application</span></span>||
| <span data-ttu-id="6f8ee-127">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="6f8ee-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6f8ee-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f8ee-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="6f8ee-129">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="6f8ee-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="6f8ee-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f8ee-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="6f8ee-131">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="6f8ee-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6f8ee-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f8ee-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6f8ee-133">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="6f8ee-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="6f8ee-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f8ee-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f8ee-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f8ee-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f8ee-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6f8ee-136">Optional query parameters</span></span>

<span data-ttu-id="6f8ee-137">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-137">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f8ee-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f8ee-138">Request headers</span></span>

|<span data-ttu-id="6f8ee-139">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f8ee-139">Header</span></span>|<span data-ttu-id="6f8ee-140">Valor</span><span class="sxs-lookup"><span data-stu-id="6f8ee-140">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f8ee-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f8ee-141">Authorization</span></span>|<span data-ttu-id="6f8ee-142">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-142">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f8ee-143">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f8ee-143">Accept</span></span>|<span data-ttu-id="6f8ee-144">application/json</span><span class="sxs-lookup"><span data-stu-id="6f8ee-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f8ee-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f8ee-145">Request body</span></span>

<span data-ttu-id="6f8ee-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f8ee-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f8ee-147">Response</span></span>

<span data-ttu-id="6f8ee-148">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-148">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f8ee-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f8ee-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f8ee-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f8ee-150">Request</span></span>

<span data-ttu-id="6f8ee-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-151">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="6f8ee-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f8ee-152">Response</span></span>

<span data-ttu-id="6f8ee-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f8ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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