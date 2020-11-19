---
title: ação createMigrationReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27a73945b3b2ba060dafef0766fa2532d42369d5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49263089"
---
# <a name="createmigrationreport-action"></a><span data-ttu-id="ac072-103">ação createMigrationReport</span><span class="sxs-lookup"><span data-stu-id="ac072-103">createMigrationReport action</span></span>

<span data-ttu-id="ac072-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac072-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac072-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac072-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac072-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac072-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac072-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ac072-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac072-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac072-108">Prerequisites</span></span>
<span data-ttu-id="ac072-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac072-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac072-111">Permission type</span></span>|<span data-ttu-id="ac072-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac072-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac072-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac072-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac072-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac072-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac072-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac072-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac072-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac072-116">Not supported.</span></span>|
|<span data-ttu-id="ac072-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac072-117">Application</span></span>|<span data-ttu-id="ac072-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac072-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac072-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac072-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/createMigrationReport
```

## <a name="request-headers"></a><span data-ttu-id="ac072-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac072-120">Request headers</span></span>
|<span data-ttu-id="ac072-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac072-121">Header</span></span>|<span data-ttu-id="ac072-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ac072-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac072-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac072-123">Authorization</span></span>|<span data-ttu-id="ac072-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac072-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac072-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac072-125">Accept</span></span>|<span data-ttu-id="ac072-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac072-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac072-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac072-127">Request body</span></span>
<span data-ttu-id="ac072-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ac072-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ac072-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ac072-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ac072-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac072-130">Property</span></span>|<span data-ttu-id="ac072-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac072-131">Type</span></span>|<span data-ttu-id="ac072-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac072-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac072-133">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="ac072-133">groupPolicyObjectFile</span></span>|[<span data-ttu-id="ac072-134">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="ac072-134">groupPolicyObjectFile</span></span>](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|<span data-ttu-id="ac072-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ac072-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ac072-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac072-136">Response</span></span>
<span data-ttu-id="ac072-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac072-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac072-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac072-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac072-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac072-139">Request</span></span>
<span data-ttu-id="ac072-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac072-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/createMigrationReport

Content-type: application/json
Content-length: 438

{
  "groupPolicyObjectFile": {
    "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
    "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
    "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "content": "Content value"
  }
}
```

### <a name="response"></a><span data-ttu-id="ac072-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac072-141">Response</span></span>
<span data-ttu-id="ac072-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac072-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Create Migration Report value"
}
```




