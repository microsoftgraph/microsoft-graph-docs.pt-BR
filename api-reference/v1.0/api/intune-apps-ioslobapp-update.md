---
title: Atualizar iosLobApp
description: Atualiza as propriedades de um objeto iosLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4609d5c967bfb6b8a65047d5f3c4af871e1f546b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516592"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="ed407-103">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="ed407-103">Update iosLobApp</span></span>

<span data-ttu-id="ed407-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed407-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed407-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed407-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed407-106">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed407-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed407-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed407-107">Prerequisites</span></span>
<span data-ttu-id="ed407-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ed407-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed407-110">Permission type</span></span>|<span data-ttu-id="ed407-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed407-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed407-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed407-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed407-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed407-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed407-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed407-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed407-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed407-115">Not supported.</span></span>|
|<span data-ttu-id="ed407-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed407-116">Application</span></span>|<span data-ttu-id="ed407-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed407-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed407-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed407-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ed407-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed407-119">Request headers</span></span>
|<span data-ttu-id="ed407-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed407-120">Header</span></span>|<span data-ttu-id="ed407-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ed407-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed407-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed407-122">Authorization</span></span>|<span data-ttu-id="ed407-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed407-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed407-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed407-124">Accept</span></span>|<span data-ttu-id="ed407-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed407-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed407-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed407-126">Request body</span></span>
<span data-ttu-id="ed407-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed407-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="ed407-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune-apps-ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="ed407-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed407-129">Property</span></span>|<span data-ttu-id="ed407-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed407-130">Type</span></span>|<span data-ttu-id="ed407-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed407-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed407-132">id</span><span class="sxs-lookup"><span data-stu-id="ed407-132">id</span></span>|<span data-ttu-id="ed407-133">String</span><span class="sxs-lookup"><span data-stu-id="ed407-133">String</span></span>|<span data-ttu-id="ed407-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ed407-134">Key of the entity.</span></span> <span data-ttu-id="ed407-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ed407-136">displayName</span></span>|<span data-ttu-id="ed407-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed407-137">String</span></span>|<span data-ttu-id="ed407-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ed407-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ed407-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-140">description</span><span class="sxs-lookup"><span data-stu-id="ed407-140">description</span></span>|<span data-ttu-id="ed407-141">String</span><span class="sxs-lookup"><span data-stu-id="ed407-141">String</span></span>|<span data-ttu-id="ed407-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed407-142">The description of the app.</span></span> <span data-ttu-id="ed407-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-144">publicador</span><span class="sxs-lookup"><span data-stu-id="ed407-144">publisher</span></span>|<span data-ttu-id="ed407-145">String</span><span class="sxs-lookup"><span data-stu-id="ed407-145">String</span></span>|<span data-ttu-id="ed407-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed407-146">The publisher of the app.</span></span> <span data-ttu-id="ed407-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ed407-148">largeIcon</span></span>|[<span data-ttu-id="ed407-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ed407-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ed407-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ed407-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ed407-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed407-152">createdDateTime</span></span>|<span data-ttu-id="ed407-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed407-153">DateTimeOffset</span></span>|<span data-ttu-id="ed407-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed407-154">The date and time the app was created.</span></span> <span data-ttu-id="ed407-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed407-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ed407-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed407-157">DateTimeOffset</span></span>|<span data-ttu-id="ed407-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ed407-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ed407-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ed407-160">isFeatured</span></span>|<span data-ttu-id="ed407-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed407-161">Boolean</span></span>|<span data-ttu-id="ed407-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ed407-163">privacyInformationUrl</span></span>|<span data-ttu-id="ed407-164">String</span><span class="sxs-lookup"><span data-stu-id="ed407-164">String</span></span>|<span data-ttu-id="ed407-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ed407-165">The privacy statement Url.</span></span> <span data-ttu-id="ed407-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ed407-167">informationUrl</span></span>|<span data-ttu-id="ed407-168">String</span><span class="sxs-lookup"><span data-stu-id="ed407-168">String</span></span>|<span data-ttu-id="ed407-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ed407-169">The more information Url.</span></span> <span data-ttu-id="ed407-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-171">owner</span><span class="sxs-lookup"><span data-stu-id="ed407-171">owner</span></span>|<span data-ttu-id="ed407-172">String</span><span class="sxs-lookup"><span data-stu-id="ed407-172">String</span></span>|<span data-ttu-id="ed407-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ed407-173">The owner of the app.</span></span> <span data-ttu-id="ed407-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-175">developer</span><span class="sxs-lookup"><span data-stu-id="ed407-175">developer</span></span>|<span data-ttu-id="ed407-176">String</span><span class="sxs-lookup"><span data-stu-id="ed407-176">String</span></span>|<span data-ttu-id="ed407-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed407-177">The developer of the app.</span></span> <span data-ttu-id="ed407-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-179">notes</span><span class="sxs-lookup"><span data-stu-id="ed407-179">notes</span></span>|<span data-ttu-id="ed407-180">String</span><span class="sxs-lookup"><span data-stu-id="ed407-180">String</span></span>|<span data-ttu-id="ed407-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed407-181">Notes for the app.</span></span> <span data-ttu-id="ed407-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ed407-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="ed407-183">publishingState</span></span>|[<span data-ttu-id="ed407-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ed407-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ed407-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed407-185">The publishing state for the app.</span></span> <span data-ttu-id="ed407-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ed407-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ed407-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed407-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ed407-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ed407-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ed407-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ed407-189">committedContentVersion</span></span>|<span data-ttu-id="ed407-190">String</span><span class="sxs-lookup"><span data-stu-id="ed407-190">String</span></span>|<span data-ttu-id="ed407-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ed407-191">The internal committed content version.</span></span> <span data-ttu-id="ed407-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ed407-193">fileName</span><span class="sxs-lookup"><span data-stu-id="ed407-193">fileName</span></span>|<span data-ttu-id="ed407-194">String</span><span class="sxs-lookup"><span data-stu-id="ed407-194">String</span></span>|<span data-ttu-id="ed407-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ed407-195">The name of the main Lob application file.</span></span> <span data-ttu-id="ed407-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ed407-197">size</span><span class="sxs-lookup"><span data-stu-id="ed407-197">size</span></span>|<span data-ttu-id="ed407-198">Int64</span><span class="sxs-lookup"><span data-stu-id="ed407-198">Int64</span></span>|<span data-ttu-id="ed407-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ed407-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="ed407-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed407-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ed407-201">bundleId</span><span class="sxs-lookup"><span data-stu-id="ed407-201">bundleId</span></span>|<span data-ttu-id="ed407-202">String</span><span class="sxs-lookup"><span data-stu-id="ed407-202">String</span></span>|<span data-ttu-id="ed407-203">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ed407-203">The Identity Name.</span></span>|
|<span data-ttu-id="ed407-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ed407-204">applicableDeviceType</span></span>|[<span data-ttu-id="ed407-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ed407-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ed407-206">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="ed407-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ed407-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ed407-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ed407-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ed407-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="ed407-209">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ed407-209">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ed407-210">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ed407-210">expirationDateTime</span></span>|<span data-ttu-id="ed407-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed407-211">DateTimeOffset</span></span>|<span data-ttu-id="ed407-212">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="ed407-212">The expiration time.</span></span>|
|<span data-ttu-id="ed407-213">versionNumber</span><span class="sxs-lookup"><span data-stu-id="ed407-213">versionNumber</span></span>|<span data-ttu-id="ed407-214">String</span><span class="sxs-lookup"><span data-stu-id="ed407-214">String</span></span>|<span data-ttu-id="ed407-215">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="ed407-215">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ed407-216">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ed407-216">buildNumber</span></span>|<span data-ttu-id="ed407-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed407-217">String</span></span>|<span data-ttu-id="ed407-218">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="ed407-218">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="ed407-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed407-219">Response</span></span>
<span data-ttu-id="ed407-220">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed407-220">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed407-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed407-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed407-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed407-222">Request</span></span>
<span data-ttu-id="ed407-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed407-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1229

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="ed407-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed407-224">Response</span></span>
<span data-ttu-id="ed407-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed407-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1401

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```




