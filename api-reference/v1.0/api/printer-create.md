---
title: 'printer: create'
description: Crie (registre) uma impressora com o serviço Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 58285c3c6908812edce8ad80915f44f4df08fcb8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516867"
---
# <a name="printer-create"></a><span data-ttu-id="7041e-103">printer: create</span><span class="sxs-lookup"><span data-stu-id="7041e-103">printer: create</span></span>
<span data-ttu-id="7041e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7041e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7041e-105">Crie (registre) uma impressora com o serviço Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="7041e-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="7041e-106">Esta é uma operação de longa duração e, como tal, retorna uma [printerCreateOperation](../resources/printercreateoperation.md) que pode ser usada para rastrear e verificar o registro da impressora.</span><span class="sxs-lookup"><span data-stu-id="7041e-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

<span data-ttu-id="7041e-107">Para ajudar a criar a CSR (Solicitação de Assinatura de Certificado) necessária para a criação da impressora, consulte o exemplo de código de geração [CSR](/universal-print/hardware/universal-print-oem-certificate-signing-request).</span><span class="sxs-lookup"><span data-stu-id="7041e-107">For help creating the required Certificate Signing Request (CSR) for creating printer, see the [CSR generation code sample](/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>

## <a name="permissions"></a><span data-ttu-id="7041e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7041e-108">Permissions</span></span>
<span data-ttu-id="7041e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7041e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7041e-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="7041e-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="7041e-112">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="7041e-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="7041e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7041e-113">Permission type</span></span> | <span data-ttu-id="7041e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7041e-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7041e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7041e-115">Delegated (work or school account)</span></span>| <span data-ttu-id="7041e-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7041e-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="7041e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7041e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7041e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7041e-118">Not Supported.</span></span>|
|<span data-ttu-id="7041e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7041e-119">Application</span></span>| <span data-ttu-id="7041e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7041e-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7041e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7041e-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/create
```

## <a name="request-headers"></a><span data-ttu-id="7041e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7041e-122">Request headers</span></span>
|<span data-ttu-id="7041e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7041e-123">Name</span></span>|<span data-ttu-id="7041e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7041e-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7041e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7041e-125">Authorization</span></span>|<span data-ttu-id="7041e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7041e-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7041e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7041e-128">Content-Type</span></span>|<span data-ttu-id="7041e-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7041e-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7041e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7041e-131">Request body</span></span>
<span data-ttu-id="7041e-132">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7041e-132">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="7041e-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7041e-133">The following table shows the parameters that can be used with this action.</span></span>

| <span data-ttu-id="7041e-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7041e-134">Parameter</span></span>      | <span data-ttu-id="7041e-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="7041e-135">Type</span></span>    |<span data-ttu-id="7041e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="7041e-136">Description</span></span>| <span data-ttu-id="7041e-137">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="7041e-137">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="7041e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7041e-138">displayName</span></span>|<span data-ttu-id="7041e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7041e-139">String</span></span>|<span data-ttu-id="7041e-140">O nome de exibição a ser atribuído à impressora.</span><span class="sxs-lookup"><span data-stu-id="7041e-140">The display name to assign to the printer.</span></span>|<span data-ttu-id="7041e-141">Sim</span><span class="sxs-lookup"><span data-stu-id="7041e-141">Yes</span></span>|
|<span data-ttu-id="7041e-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="7041e-142">manufacturer</span></span>|<span data-ttu-id="7041e-143">String</span><span class="sxs-lookup"><span data-stu-id="7041e-143">String</span></span>|<span data-ttu-id="7041e-144">O fabricante da impressora.</span><span class="sxs-lookup"><span data-stu-id="7041e-144">The manufacturer of the printer.</span></span>|<span data-ttu-id="7041e-145">Sim</span><span class="sxs-lookup"><span data-stu-id="7041e-145">Yes</span></span>|
|<span data-ttu-id="7041e-146">modelo</span><span class="sxs-lookup"><span data-stu-id="7041e-146">model</span></span>|<span data-ttu-id="7041e-147">String</span><span class="sxs-lookup"><span data-stu-id="7041e-147">String</span></span>|<span data-ttu-id="7041e-148">O modelo da impressora.</span><span class="sxs-lookup"><span data-stu-id="7041e-148">The model of the printer.</span></span>|<span data-ttu-id="7041e-149">Sim</span><span class="sxs-lookup"><span data-stu-id="7041e-149">Yes</span></span>|
|<span data-ttu-id="7041e-150">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="7041e-150">physicalDeviceId</span></span>|<span data-ttu-id="7041e-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7041e-151">String</span></span>|<span data-ttu-id="7041e-152">O UUID do dispositivo físico da impressora.</span><span class="sxs-lookup"><span data-stu-id="7041e-152">The physical device UUID of the printer.</span></span> <span data-ttu-id="7041e-153">Obrigatório se a `hasPhysicalDevice` propriedade for true.</span><span class="sxs-lookup"><span data-stu-id="7041e-153">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="7041e-154">Não</span><span class="sxs-lookup"><span data-stu-id="7041e-154">No</span></span>|
|<span data-ttu-id="7041e-155">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="7041e-155">hasPhysicalDevice</span></span>|<span data-ttu-id="7041e-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="7041e-156">Boolean</span></span>|<span data-ttu-id="7041e-157">True se a impressora tiver um dispositivo de saída físico, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="7041e-157">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="7041e-158">Se omitido, o valor padrão será true.</span><span class="sxs-lookup"><span data-stu-id="7041e-158">If omitted, the default value is true.</span></span>|<span data-ttu-id="7041e-159">Não</span><span class="sxs-lookup"><span data-stu-id="7041e-159">No</span></span>|
|<span data-ttu-id="7041e-160">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="7041e-160">certificateSigningRequest</span></span>|[<span data-ttu-id="7041e-161">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="7041e-161">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="7041e-162">A Solicitação de Assinatura de Certificado X.509 (CSR) para o certificado criado e usado pela impressora para se identificar.</span><span class="sxs-lookup"><span data-stu-id="7041e-162">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="7041e-163">Sim</span><span class="sxs-lookup"><span data-stu-id="7041e-163">Yes</span></span>|
|<span data-ttu-id="7041e-164">connectorId</span><span class="sxs-lookup"><span data-stu-id="7041e-164">connectorId</span></span>|<span data-ttu-id="7041e-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7041e-165">String</span></span>|<span data-ttu-id="7041e-166">ID do conector atuando como proxy para a impressora.</span><span class="sxs-lookup"><span data-stu-id="7041e-166">ID of the connector acting as proxy to the printer.</span></span>|<span data-ttu-id="7041e-167">Não</span><span class="sxs-lookup"><span data-stu-id="7041e-167">No</span></span>|

## <a name="response"></a><span data-ttu-id="7041e-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="7041e-168">Response</span></span>
<span data-ttu-id="7041e-169">Se tiver êxito, este método retornará um código de resposta e um link para `202 Accepted` a [impressora associadaCreateOperation](../resources/printercreateoperation.md) no `Operation-Location` header.</span><span class="sxs-lookup"><span data-stu-id="7041e-169">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="7041e-170">Você faz uma solicitação GET para a URL vinculada para obter o status de um registro de impressora em andamento.</span><span class="sxs-lookup"><span data-stu-id="7041e-170">You make a GET request to the linked URL to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="7041e-171">Depois que o registro da impressora for concluído com êxito, uma solicitação GET para a URL vinculada conterá o objeto de impressora criado e o certificado registrado.</span><span class="sxs-lookup"><span data-stu-id="7041e-171">After printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="7041e-172">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7041e-172">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7041e-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7041e-173">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printer_create"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/create
Content-Type: application/json
Content-length: 287

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```


### <a name="response"></a><span data-ttu-id="7041e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="7041e-174">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/v1.0/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

