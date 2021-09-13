---
title: tipo de número browserSyncSetting
description: Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cfaec7d41ae18d12ad4801fdc1110250d6288b62
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127483"
---
# <a name="browsersyncsetting-enum-type"></a>tipo de número browserSyncSetting

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Padrão – Permitir a sincronização das configurações do navegador entre dispositivos.|
|blockedWithUserOverride|1|Impedir a sincronização das configurações do navegador entre dispositivos do usuário, permitir a substituição do usuário da configuração.|
|blocked|2|Impedir absolutamente a sincronização das configurações do navegador em dispositivos de usuário.|



