---
title: Listar managedAppOperations
description: Listar propriedades e relações de objetos de managedAppOperation.
ms.openlocfilehash: f858a0a70b7c97321a4d6d503b238363253624f7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038336"
---
# <a name="list-managedappoperations"></a><span data-ttu-id="f99cf-103">Listar managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="f99cf-103">List managedAppOperations</span></span>

> <span data-ttu-id="f99cf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f99cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f99cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f99cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f99cf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f99cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f99cf-107">Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="f99cf-107">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f99cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f99cf-108">Prerequisites</span></span>
<span data-ttu-id="f99cf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f99cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f99cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f99cf-111">Permission type</span></span>|<span data-ttu-id="f99cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f99cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f99cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f99cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f99cf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f99cf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f99cf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f99cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f99cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f99cf-116">Not supported.</span></span>|
|<span data-ttu-id="f99cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f99cf-117">Application</span></span>|<span data-ttu-id="f99cf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f99cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f99cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f99cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="f99cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f99cf-120">Request headers</span></span>
|<span data-ttu-id="f99cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f99cf-121">Header</span></span>|<span data-ttu-id="f99cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f99cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f99cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f99cf-123">Authorization</span></span>|<span data-ttu-id="f99cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f99cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f99cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f99cf-125">Accept</span></span>|<span data-ttu-id="f99cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f99cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f99cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f99cf-127">Request body</span></span>
<span data-ttu-id="f99cf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f99cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f99cf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f99cf-129">Response</span></span>
<span data-ttu-id="f99cf-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f99cf-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f99cf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f99cf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f99cf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f99cf-132">Request</span></span>
<span data-ttu-id="f99cf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f99cf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="f99cf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f99cf-134">Response</span></span>
<span data-ttu-id="f99cf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f99cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppOperation",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "State value",
      "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
      "version": "Version value"
    }
  ]
}
```





