---
title: Função getManagedAppPolicies
description: Obtém as restrições de aplicativo para um determinado usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93161a696d572742d820074fcded9a537ea47ea1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725851"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="01b0a-103">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="01b0a-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="01b0a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01b0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01b0a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01b0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01b0a-106">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="01b0a-106">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01b0a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01b0a-107">Prerequisites</span></span>
<span data-ttu-id="01b0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01b0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01b0a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01b0a-110">Permission type</span></span>|<span data-ttu-id="01b0a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01b0a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01b0a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01b0a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01b0a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b0a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="01b0a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01b0a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01b0a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01b0a-115">Not supported.</span></span>|
|<span data-ttu-id="01b0a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01b0a-116">Application</span></span>|<span data-ttu-id="01b0a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01b0a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01b0a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01b0a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="01b0a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01b0a-119">Request headers</span></span>
|<span data-ttu-id="01b0a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01b0a-120">Header</span></span>|<span data-ttu-id="01b0a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="01b0a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01b0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="01b0a-122">Authorization</span></span>|<span data-ttu-id="01b0a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01b0a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01b0a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01b0a-124">Accept</span></span>|<span data-ttu-id="01b0a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01b0a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01b0a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01b0a-126">Request body</span></span>
<span data-ttu-id="01b0a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01b0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01b0a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="01b0a-128">Response</span></span>
<span data-ttu-id="01b0a-129">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01b0a-129">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01b0a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01b0a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="01b0a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01b0a-131">Request</span></span>
<span data-ttu-id="01b0a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01b0a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="01b0a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="01b0a-133">Response</span></span>
<span data-ttu-id="01b0a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01b0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```





