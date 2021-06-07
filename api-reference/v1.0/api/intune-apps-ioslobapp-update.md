---
title: Atualizar iosLobApp
description: Atualiza as propriedades de um objeto iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77f9689028ad50d0004670e31dda80b7a90babd5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757392"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="789d8-103">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="789d8-103">Update iosLobApp</span></span>

<span data-ttu-id="789d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="789d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="789d8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="789d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="789d8-106">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="789d8-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="789d8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="789d8-107">Prerequisites</span></span>
<span data-ttu-id="789d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="789d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="789d8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="789d8-110">Permission type</span></span>|<span data-ttu-id="789d8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="789d8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="789d8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="789d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="789d8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789d8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="789d8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="789d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="789d8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="789d8-115">Not supported.</span></span>|
|<span data-ttu-id="789d8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="789d8-116">Application</span></span>|<span data-ttu-id="789d8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789d8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="789d8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="789d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="789d8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="789d8-119">Request headers</span></span>
|<span data-ttu-id="789d8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="789d8-120">Header</span></span>|<span data-ttu-id="789d8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="789d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="789d8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="789d8-122">Authorization</span></span>|<span data-ttu-id="789d8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="789d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="789d8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="789d8-124">Accept</span></span>|<span data-ttu-id="789d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="789d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="789d8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="789d8-126">Request body</span></span>
<span data-ttu-id="789d8-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="789d8-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="789d8-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune-apps-ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="789d8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="789d8-129">Property</span></span>|<span data-ttu-id="789d8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="789d8-130">Type</span></span>|<span data-ttu-id="789d8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="789d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="789d8-132">id</span><span class="sxs-lookup"><span data-stu-id="789d8-132">id</span></span>|<span data-ttu-id="789d8-133">String</span><span class="sxs-lookup"><span data-stu-id="789d8-133">String</span></span>|<span data-ttu-id="789d8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="789d8-134">Key of the entity.</span></span> <span data-ttu-id="789d8-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="789d8-136">displayName</span></span>|<span data-ttu-id="789d8-137">String</span><span class="sxs-lookup"><span data-stu-id="789d8-137">String</span></span>|<span data-ttu-id="789d8-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="789d8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="789d8-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-140">description</span><span class="sxs-lookup"><span data-stu-id="789d8-140">description</span></span>|<span data-ttu-id="789d8-141">String</span><span class="sxs-lookup"><span data-stu-id="789d8-141">String</span></span>|<span data-ttu-id="789d8-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="789d8-142">The description of the app.</span></span> <span data-ttu-id="789d8-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-144">publicador</span><span class="sxs-lookup"><span data-stu-id="789d8-144">publisher</span></span>|<span data-ttu-id="789d8-145">String</span><span class="sxs-lookup"><span data-stu-id="789d8-145">String</span></span>|<span data-ttu-id="789d8-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="789d8-146">The publisher of the app.</span></span> <span data-ttu-id="789d8-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="789d8-148">largeIcon</span></span>|[<span data-ttu-id="789d8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="789d8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="789d8-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="789d8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="789d8-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="789d8-152">createdDateTime</span></span>|<span data-ttu-id="789d8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="789d8-153">DateTimeOffset</span></span>|<span data-ttu-id="789d8-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="789d8-154">The date and time the app was created.</span></span> <span data-ttu-id="789d8-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="789d8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="789d8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="789d8-157">DateTimeOffset</span></span>|<span data-ttu-id="789d8-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="789d8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="789d8-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="789d8-160">isFeatured</span></span>|<span data-ttu-id="789d8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="789d8-161">Boolean</span></span>|<span data-ttu-id="789d8-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="789d8-163">privacyInformationUrl</span></span>|<span data-ttu-id="789d8-164">String</span><span class="sxs-lookup"><span data-stu-id="789d8-164">String</span></span>|<span data-ttu-id="789d8-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="789d8-165">The privacy statement Url.</span></span> <span data-ttu-id="789d8-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="789d8-167">informationUrl</span></span>|<span data-ttu-id="789d8-168">String</span><span class="sxs-lookup"><span data-stu-id="789d8-168">String</span></span>|<span data-ttu-id="789d8-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="789d8-169">The more information Url.</span></span> <span data-ttu-id="789d8-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="789d8-171">owner</span></span>|<span data-ttu-id="789d8-172">String</span><span class="sxs-lookup"><span data-stu-id="789d8-172">String</span></span>|<span data-ttu-id="789d8-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="789d8-173">The owner of the app.</span></span> <span data-ttu-id="789d8-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-175">developer</span><span class="sxs-lookup"><span data-stu-id="789d8-175">developer</span></span>|<span data-ttu-id="789d8-176">String</span><span class="sxs-lookup"><span data-stu-id="789d8-176">String</span></span>|<span data-ttu-id="789d8-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="789d8-177">The developer of the app.</span></span> <span data-ttu-id="789d8-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-179">notes</span><span class="sxs-lookup"><span data-stu-id="789d8-179">notes</span></span>|<span data-ttu-id="789d8-180">String</span><span class="sxs-lookup"><span data-stu-id="789d8-180">String</span></span>|<span data-ttu-id="789d8-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="789d8-181">Notes for the app.</span></span> <span data-ttu-id="789d8-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="789d8-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="789d8-183">publishingState</span></span>|[<span data-ttu-id="789d8-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="789d8-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="789d8-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="789d8-185">The publishing state for the app.</span></span> <span data-ttu-id="789d8-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="789d8-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="789d8-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="789d8-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="789d8-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="789d8-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="789d8-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="789d8-189">committedContentVersion</span></span>|<span data-ttu-id="789d8-190">String</span><span class="sxs-lookup"><span data-stu-id="789d8-190">String</span></span>|<span data-ttu-id="789d8-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="789d8-191">The internal committed content version.</span></span> <span data-ttu-id="789d8-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="789d8-193">fileName</span><span class="sxs-lookup"><span data-stu-id="789d8-193">fileName</span></span>|<span data-ttu-id="789d8-194">String</span><span class="sxs-lookup"><span data-stu-id="789d8-194">String</span></span>|<span data-ttu-id="789d8-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="789d8-195">The name of the main Lob application file.</span></span> <span data-ttu-id="789d8-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="789d8-197">size</span><span class="sxs-lookup"><span data-stu-id="789d8-197">size</span></span>|<span data-ttu-id="789d8-198">Int64</span><span class="sxs-lookup"><span data-stu-id="789d8-198">Int64</span></span>|<span data-ttu-id="789d8-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="789d8-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="789d8-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="789d8-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="789d8-201">bundleId</span><span class="sxs-lookup"><span data-stu-id="789d8-201">bundleId</span></span>|<span data-ttu-id="789d8-202">String</span><span class="sxs-lookup"><span data-stu-id="789d8-202">String</span></span>|<span data-ttu-id="789d8-203">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="789d8-203">The Identity Name.</span></span>|
|<span data-ttu-id="789d8-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="789d8-204">applicableDeviceType</span></span>|[<span data-ttu-id="789d8-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="789d8-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="789d8-206">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="789d8-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="789d8-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="789d8-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="789d8-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="789d8-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="789d8-209">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="789d8-209">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="789d8-210">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="789d8-210">expirationDateTime</span></span>|<span data-ttu-id="789d8-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="789d8-211">DateTimeOffset</span></span>|<span data-ttu-id="789d8-212">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="789d8-212">The expiration time.</span></span>|
|<span data-ttu-id="789d8-213">versionNumber</span><span class="sxs-lookup"><span data-stu-id="789d8-213">versionNumber</span></span>|<span data-ttu-id="789d8-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="789d8-214">String</span></span>|<span data-ttu-id="789d8-215">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="789d8-215">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="789d8-216">buildNumber</span><span class="sxs-lookup"><span data-stu-id="789d8-216">buildNumber</span></span>|<span data-ttu-id="789d8-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="789d8-217">String</span></span>|<span data-ttu-id="789d8-218">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="789d8-218">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="789d8-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="789d8-219">Response</span></span>
<span data-ttu-id="789d8-220">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="789d8-220">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="789d8-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="789d8-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="789d8-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="789d8-222">Request</span></span>
<span data-ttu-id="789d8-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="789d8-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1249

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="789d8-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="789d8-224">Response</span></span>
<span data-ttu-id="789d8-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="789d8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1421

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```




