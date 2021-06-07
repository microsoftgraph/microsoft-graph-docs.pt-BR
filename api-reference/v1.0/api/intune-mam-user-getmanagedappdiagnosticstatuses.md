---
title: função getManagedAppDiagnosticStatuses
description: Obtém diagnóstico do status de validação para um determinado usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 754c1821324fc4c5f0c9c38301c2f1528238c150
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751741"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="3ab25-103">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="3ab25-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="3ab25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ab25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ab25-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ab25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ab25-106">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="3ab25-106">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ab25-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ab25-107">Prerequisites</span></span>
<span data-ttu-id="3ab25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ab25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ab25-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ab25-110">Permission type</span></span>|<span data-ttu-id="3ab25-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ab25-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ab25-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ab25-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ab25-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ab25-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ab25-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ab25-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ab25-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ab25-115">Not supported.</span></span>|
|<span data-ttu-id="3ab25-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ab25-116">Application</span></span>|<span data-ttu-id="3ab25-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ab25-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ab25-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ab25-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="3ab25-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ab25-119">Request headers</span></span>
|<span data-ttu-id="3ab25-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ab25-120">Header</span></span>|<span data-ttu-id="3ab25-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3ab25-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ab25-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ab25-122">Authorization</span></span>|<span data-ttu-id="3ab25-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ab25-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ab25-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ab25-124">Accept</span></span>|<span data-ttu-id="3ab25-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ab25-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ab25-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ab25-126">Request body</span></span>
<span data-ttu-id="3ab25-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ab25-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ab25-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ab25-128">Response</span></span>
<span data-ttu-id="3ab25-129">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ab25-129">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ab25-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ab25-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ab25-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ab25-131">Request</span></span>
<span data-ttu-id="3ab25-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ab25-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="3ab25-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ab25-133">Response</span></span>
<span data-ttu-id="3ab25-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ab25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




