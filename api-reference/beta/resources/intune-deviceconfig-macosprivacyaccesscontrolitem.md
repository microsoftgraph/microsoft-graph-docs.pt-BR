---
title: Tipo de recurso macOSPrivacyAccessControlItem
description: Representa as preferências de privacidade por processo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be98e81399edc9682797f1b1aa7f04d1f02803bf
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669067"
---
# <a name="macosprivacyaccesscontrolitem-resource-type"></a>Tipo de recurso macOSPrivacyAccessControlItem

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa as preferências de privacidade por processo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do aplicativo, processo ou executável.|
|identificador|Cadeia de Caracteres|A ID do pacote ou o caminho do aplicativo, processo ou executável.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Uma ID de pacote é usada para identificar um aplicativo. Um caminho é usado para identificar um processo ou executável. Os valores possíveis são: `bundleID` e `path`.|
|codeRequirement|Cadeia de Caracteres|Insira o requisito de código, que pode ser obtido com o comando 'codesign –display -r –' no aplicativo Terminal. Inclua tudo após '=>'.|
|staticCodeValidation|Boolean|Valida estaticamente o requisito de código. Use essa configuração se o processo invalidar sua assinatura de código dinâmico.|
|blockCamera|Booleano|Bloquear o acesso ao aplicativo de câmera.|
|blockMicrophone|Booleano|Bloquear o acesso ao microfone.|
|blockScreenCapture|Booleano|Impedir que o aplicativo capture o conteúdo da exibição do sistema. Requer o macOS 10.15 ou posterior.|
|blockListenEvent|Booleano|Impedir que o aplicativo ou o processo ouça eventos de dispositivos de entrada, como mouse, teclado e trackpad. Requer o macOS 10.15 ou posterior.|
|speechRecognition|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso ao recurso de reconhecimento de fala do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Acessibilidade|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir que o aplicativo ou processo controle o Mac por meio do subsistema acessibilidade. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Addressbook|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso a informações de contato gerenciadas por Contatos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|calendar|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso a informações de evento gerenciadas pelo Calendário. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Lembretes|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso a informações gerenciadas por Lembretes. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|fotos|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso a imagens gerenciadas por Fotos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|mediaLibrary|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso à música e à biblioteca de mídia. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|fileProviderPresence|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir que o aplicativo ou processo acesse arquivos gerenciados pela extensão do provedor de arquivos de outro aplicativo. Requer o macOS 10.15 ou posterior. . Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyAllFiles|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Controlar o acesso a todos os arquivos protegidos em um dispositivo. Os arquivos podem estar em locais como emails, mensagens, aplicativos e configurações administrativas. Aplique essa configuração com cuidado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicySystemAdminFiles|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir que o aplicativo ou o processo acesse os arquivos usados na administração do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDesktopFolder|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso à pasta Área de Trabalho. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDocumentsFolder|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso à pasta Documentos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDownloadsFolder|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso à pasta Downloads. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyNetworkVolumes|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Permitir ou bloquear o acesso a volumes de rede. Requer o macOS 10.15 ou posterior. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyRemovableVolumes|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Controlar o acesso a volumes removíveis no dispositivo, como um disco rígido externo. Requer o macOS 10.15 ou posterior. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|postEvent|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Controlar o acesso às APIs CoreGraphics, que são usadas para enviar CGEvents para o fluxo de eventos do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|appleEventsAllowedReceivers|[Coleção macOSAppleEventReceiver](../resources/intune-deviceconfig-macosappleeventreceiver.md)|Permitir ou negar que o aplicativo ou processo envie um evento apple restrito para outro aplicativo ou processo. Você precisará saber o identificador, o tipo de identificador e o requisito de código do aplicativo ou processo de recebimento. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSPrivacyAccessControlItem",
  "displayName": "String",
  "identifier": "String",
  "identifierType": "String",
  "codeRequirement": "String",
  "staticCodeValidation": true,
  "blockCamera": true,
  "blockMicrophone": true,
  "blockScreenCapture": true,
  "blockListenEvent": true,
  "speechRecognition": "String",
  "accessibility": "String",
  "addressBook": "String",
  "calendar": "String",
  "reminders": "String",
  "photos": "String",
  "mediaLibrary": "String",
  "fileProviderPresence": "String",
  "systemPolicyAllFiles": "String",
  "systemPolicySystemAdminFiles": "String",
  "systemPolicyDesktopFolder": "String",
  "systemPolicyDocumentsFolder": "String",
  "systemPolicyDownloadsFolder": "String",
  "systemPolicyNetworkVolumes": "String",
  "systemPolicyRemovableVolumes": "String",
  "postEvent": "String",
  "appleEventsAllowedReceivers": [
    {
      "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
      "codeRequirement": "String",
      "identifier": "String",
      "identifierType": "String",
      "allowed": true
    }
  ]
}
```




