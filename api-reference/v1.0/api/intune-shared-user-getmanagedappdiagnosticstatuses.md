---
title: função getManagedAppDiagnosticStatuses
description: Obtém diagnóstico do status de validação para um determinado usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ea68ef093283f68e1cf7460c3a731c369c6e9955
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950575"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="e6287-103">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="e6287-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="e6287-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e6287-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6287-105">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="e6287-105">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6287-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6287-106">Prerequisites</span></span>
<span data-ttu-id="e6287-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6287-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6287-109">Permission type</span></span>|<span data-ttu-id="e6287-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6287-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6287-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6287-111">Delegated (work or school account)</span></span>| <span data-ttu-id="e6287-112">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="e6287-112">_varies by context_</span></span>|
| <span data-ttu-id="e6287-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="e6287-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="e6287-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6287-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="e6287-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6287-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6287-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6287-116">Not supported.</span></span>|
|<span data-ttu-id="e6287-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6287-117">Application</span></span>|<span data-ttu-id="e6287-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6287-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6287-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6287-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e6287-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6287-120">Request headers</span></span>
|<span data-ttu-id="e6287-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6287-121">Header</span></span>|<span data-ttu-id="e6287-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e6287-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6287-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6287-123">Authorization</span></span>|<span data-ttu-id="e6287-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6287-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6287-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6287-125">Accept</span></span>|<span data-ttu-id="e6287-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6287-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6287-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6287-127">Request body</span></span>
<span data-ttu-id="e6287-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6287-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6287-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6287-129">Response</span></span>
<span data-ttu-id="e6287-130">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6287-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6287-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6287-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6287-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6287-132">Request</span></span>
<span data-ttu-id="e6287-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6287-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="e6287-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6287-134">Response</span></span>
<span data-ttu-id="e6287-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6287-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



