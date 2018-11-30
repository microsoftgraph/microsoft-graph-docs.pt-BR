---
title: função getManagedAppDiagnosticStatuses
description: Obtém diagnóstico do status de validação para um determinado usuário.
ms.openlocfilehash: 9ba27e90de7faff043e1acbb755bc2c9d36c43fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006449"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="395e9-103">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="395e9-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="395e9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="395e9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="395e9-105">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="395e9-105">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="395e9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="395e9-106">Prerequisites</span></span>
<span data-ttu-id="395e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="395e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="395e9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="395e9-109">Permission type</span></span>|<span data-ttu-id="395e9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="395e9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="395e9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="395e9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="395e9-112">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="395e9-112">_varies by context_</span></span>|
| <span data-ttu-id="395e9-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="395e9-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="395e9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="395e9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="395e9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="395e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="395e9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="395e9-116">Not supported.</span></span>|
|<span data-ttu-id="395e9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="395e9-117">Application</span></span>|<span data-ttu-id="395e9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="395e9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="395e9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="395e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="395e9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="395e9-120">Request headers</span></span>
|<span data-ttu-id="395e9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="395e9-121">Header</span></span>|<span data-ttu-id="395e9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="395e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="395e9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="395e9-123">Authorization</span></span>|<span data-ttu-id="395e9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="395e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="395e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="395e9-125">Accept</span></span>|<span data-ttu-id="395e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="395e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="395e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="395e9-127">Request body</span></span>
<span data-ttu-id="395e9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="395e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="395e9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="395e9-129">Response</span></span>
<span data-ttu-id="395e9-130">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="395e9-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="395e9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="395e9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="395e9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="395e9-132">Request</span></span>
<span data-ttu-id="395e9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="395e9-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="395e9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="395e9-134">Response</span></span>
<span data-ttu-id="395e9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="395e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



