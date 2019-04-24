---
title: Criar termsAndConditionsAcceptanceStatus
description: Cria um novo objeto termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 086d84a79a593dc04b6975ea3e46809a9f1c8d21
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32482918"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="e8411-103">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e8411-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="e8411-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8411-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8411-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8411-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8411-106">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="e8411-106">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8411-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8411-107">Prerequisites</span></span>
<span data-ttu-id="e8411-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8411-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8411-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8411-110">Permission type</span></span>|<span data-ttu-id="e8411-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8411-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8411-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8411-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8411-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8411-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8411-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8411-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8411-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8411-115">Not supported.</span></span>|
|<span data-ttu-id="e8411-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8411-116">Application</span></span>|<span data-ttu-id="e8411-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8411-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8411-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8411-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e8411-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8411-119">Request headers</span></span>
|<span data-ttu-id="e8411-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8411-120">Header</span></span>|<span data-ttu-id="e8411-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e8411-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8411-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8411-122">Authorization</span></span>|<span data-ttu-id="e8411-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8411-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8411-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8411-124">Accept</span></span>|<span data-ttu-id="e8411-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8411-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8411-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8411-126">Request body</span></span>
<span data-ttu-id="e8411-127">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="e8411-127">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="e8411-128">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="e8411-128">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="e8411-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8411-129">Property</span></span>|<span data-ttu-id="e8411-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8411-130">Type</span></span>|<span data-ttu-id="e8411-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8411-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8411-132">id</span><span class="sxs-lookup"><span data-stu-id="e8411-132">id</span></span>|<span data-ttu-id="e8411-133">String</span><span class="sxs-lookup"><span data-stu-id="e8411-133">String</span></span>|<span data-ttu-id="e8411-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="e8411-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e8411-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e8411-135">userDisplayName</span></span>|<span data-ttu-id="e8411-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8411-136">String</span></span>|<span data-ttu-id="e8411-137">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="e8411-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="e8411-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="e8411-138">acceptedVersion</span></span>|<span data-ttu-id="e8411-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e8411-139">Int32</span></span>|<span data-ttu-id="e8411-140">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="e8411-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="e8411-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8411-141">acceptedDateTime</span></span>|<span data-ttu-id="e8411-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8411-142">DateTimeOffset</span></span>|<span data-ttu-id="e8411-143">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="e8411-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="e8411-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8411-144">Response</span></span>
<span data-ttu-id="e8411-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8411-145">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8411-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8411-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8411-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8411-147">Request</span></span>
<span data-ttu-id="e8411-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8411-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e8411-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8411-149">Response</span></span>
<span data-ttu-id="e8411-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8411-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```





