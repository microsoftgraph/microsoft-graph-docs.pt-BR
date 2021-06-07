---
title: Criar termsAndConditionsAcceptanceStatus
description: Cria um novo objeto termsAndConditionsAcceptanceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec1b815b86e9ce7618dfdd5f66b32c9dd7737bb0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759389"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="fe5f1-103">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fe5f1-103">Create termsAndConditionsAcceptanceStatus</span></span>

<span data-ttu-id="fe5f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe5f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe5f1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe5f1-106">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="fe5f1-106">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe5f1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe5f1-107">Prerequisites</span></span>
<span data-ttu-id="fe5f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe5f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe5f1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe5f1-110">Permission type</span></span>|<span data-ttu-id="fe5f1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe5f1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe5f1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe5f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe5f1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe5f1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fe5f1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe5f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe5f1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-115">Not supported.</span></span>|
|<span data-ttu-id="fe5f1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe5f1-116">Application</span></span>|<span data-ttu-id="fe5f1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe5f1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe5f1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe5f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="fe5f1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe5f1-119">Request headers</span></span>
|<span data-ttu-id="fe5f1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe5f1-120">Header</span></span>|<span data-ttu-id="fe5f1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fe5f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe5f1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe5f1-122">Authorization</span></span>|<span data-ttu-id="fe5f1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe5f1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe5f1-124">Accept</span></span>|<span data-ttu-id="fe5f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe5f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe5f1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe5f1-126">Request body</span></span>
<span data-ttu-id="fe5f1-127">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-127">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="fe5f1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-128">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="fe5f1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe5f1-129">Property</span></span>|<span data-ttu-id="fe5f1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe5f1-130">Type</span></span>|<span data-ttu-id="fe5f1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe5f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe5f1-132">id</span><span class="sxs-lookup"><span data-stu-id="fe5f1-132">id</span></span>|<span data-ttu-id="fe5f1-133">String</span><span class="sxs-lookup"><span data-stu-id="fe5f1-133">String</span></span>|<span data-ttu-id="fe5f1-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="fe5f1-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fe5f1-135">userDisplayName</span></span>|<span data-ttu-id="fe5f1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe5f1-136">String</span></span>|<span data-ttu-id="fe5f1-137">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="fe5f1-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="fe5f1-138">acceptedVersion</span></span>|<span data-ttu-id="fe5f1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="fe5f1-139">Int32</span></span>|<span data-ttu-id="fe5f1-140">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="fe5f1-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe5f1-141">acceptedDateTime</span></span>|<span data-ttu-id="fe5f1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe5f1-142">DateTimeOffset</span></span>|<span data-ttu-id="fe5f1-143">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-143">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="fe5f1-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe5f1-144">userPrincipalName</span></span>|<span data-ttu-id="fe5f1-145">String</span><span class="sxs-lookup"><span data-stu-id="fe5f1-145">String</span></span>|<span data-ttu-id="fe5f1-146">O userPrincipalName do Usuário que aceitou o termo.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-146">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="fe5f1-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe5f1-147">Response</span></span>
<span data-ttu-id="fe5f1-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-148">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe5f1-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe5f1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe5f1-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe5f1-150">Request</span></span>
<span data-ttu-id="fe5f1-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="fe5f1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe5f1-152">Response</span></span>
<span data-ttu-id="fe5f1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




