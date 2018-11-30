---
title: função getManagedAppDiagnosticStatuses
description: Obtém diagnóstico do status de validação para um determinado usuário.
ms.openlocfilehash: bbbb399ef26c38972f989c2e1129fe61baffa0fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039660"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="92b90-103">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="92b90-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="92b90-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92b90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92b90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92b90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92b90-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="92b90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92b90-107">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="92b90-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92b90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92b90-108">Prerequisites</span></span>
<span data-ttu-id="92b90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92b90-111">Permission type</span></span>|<span data-ttu-id="92b90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92b90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92b90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92b90-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="92b90-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="92b90-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="92b90-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b90-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="92b90-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92b90-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92b90-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92b90-117">Not supported.</span></span>|
|<span data-ttu-id="92b90-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92b90-118">Application</span></span>|<span data-ttu-id="92b90-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92b90-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92b90-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92b90-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="92b90-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92b90-121">Request headers</span></span>
|<span data-ttu-id="92b90-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92b90-122">Header</span></span>|<span data-ttu-id="92b90-123">Valor</span><span class="sxs-lookup"><span data-stu-id="92b90-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92b90-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="92b90-124">Authorization</span></span>|<span data-ttu-id="92b90-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92b90-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92b90-126">Accept</span><span class="sxs-lookup"><span data-stu-id="92b90-126">Accept</span></span>|<span data-ttu-id="92b90-127">application/json</span><span class="sxs-lookup"><span data-stu-id="92b90-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b90-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92b90-128">Request body</span></span>
<span data-ttu-id="92b90-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92b90-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92b90-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="92b90-130">Response</span></span>
<span data-ttu-id="92b90-131">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92b90-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92b90-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92b90-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="92b90-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92b90-133">Request</span></span>
<span data-ttu-id="92b90-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92b90-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="92b90-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="92b90-135">Response</span></span>
<span data-ttu-id="92b90-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92b90-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






